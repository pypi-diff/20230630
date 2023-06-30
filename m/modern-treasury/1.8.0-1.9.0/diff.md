# Comparing `tmp/modern_treasury-1.8.0.tar.gz` & `tmp/modern_treasury-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modern_treasury-1.8.0.tar", max compression
+gzip compressed data, was "modern_treasury-1.9.0.tar", max compression
```

## Comparing `modern_treasury-1.8.0.tar` & `modern_treasury-1.9.0.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0     1055 2023-03-06 20:55:45.043854 modern_treasury-1.8.0/LICENSE
--rw-r--r--   0        0        0    16749 2023-03-06 20:55:45.543854 modern_treasury-1.8.0/README.md
--rw-r--r--   0        0        0     1644 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1781 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/__init__.py
--rw-r--r--   0        0        0    36088 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_base_client.py
--rw-r--r--   0        0        0     3889 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_base_exceptions.py
--rw-r--r--   0        0        0    19928 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_client.py
--rw-r--r--   0        0        0      723 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_exceptions.py
--rw-r--r--   0        0        0     6733 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/_models.py
--rw-r--r--   0        0        0     4781 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_qs.py
--rw-r--r--   0        0        0      926 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_resource.py
--rw-r--r--   0        0        0     3961 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_types.py
--rw-r--r--   0        0        0     1126 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/_utils/__init__.py
--rw-r--r--   0        0        0     3810 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/_utils/_transform.py
--rw-r--r--   0        0        0     9047 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/_utils/_utils.py
--rw-r--r--   0        0        0      106 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/_version.py
--rw-r--r--   0        0        0     2010 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/pagination.py
--rw-r--r--   0        0        0        0 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/py.typed
--rw-r--r--   0        0        0     2864 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/resources/__init__.py
--rw-r--r--   0        0        0    10299 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/account_details.py
--rw-r--r--   0        0        0     3795 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/connections.py
--rw-r--r--   0        0        0    24302 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/counterparties.py
--rw-r--r--   0        0        0    10162 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/documents.py
--rw-r--r--   0        0        0     5651 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/events.py
--rw-r--r--   0        0        0    27798 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/expected_payments.py
--rw-r--r--   0        0        0    24446 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/external_accounts.py
--rw-r--r--   0        0        0    15550 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/incoming_payment_details.py
--rw-r--r--   0        0        0      288 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/resources/internal_accounts/__init__.py
--rw-r--r--   0        0        0     6010 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/internal_accounts/balance_reports.py
--rw-r--r--   0        0        0    15922 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/internal_accounts/internal_accounts.py
--rw-r--r--   0        0        0    24038 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_account_categories.py
--rw-r--r--   0        0        0    13561 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_account_payouts.py
--rw-r--r--   0        0        0    18026 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_accounts.py
--rw-r--r--   0        0        0    10279 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_entries.py
--rw-r--r--   0        0        0      267 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_transactions/__init__.py
--rw-r--r--   0        0        0    19841 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_transactions/ledger_transactions.py
--rw-r--r--   0        0        0     8273 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledger_transactions/versions.py
--rw-r--r--   0        0        0    12957 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/ledgers.py
--rw-r--r--   0        0        0     7605 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/line_items.py
--rw-r--r--   0        0        0     5909 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/paper_items.py
--rw-r--r--   0        0        0      247 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/resources/payment_orders/__init__.py
--rw-r--r--   0        0        0    83984 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/payment_orders/payment_orders.py
--rw-r--r--   0        0        0     9243 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/payment_orders/reversals.py
--rw-r--r--   0        0        0     6213 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/payment_references.py
--rw-r--r--   0        0        0    13327 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/returns.py
--rw-r--r--   0        0        0    11753 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/routing_details.py
--rw-r--r--   0        0        0    10809 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/transactions.py
--rw-r--r--   0        0        0     4135 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/validations.py
--rw-r--r--   0        0        0    15852 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/resources/virtual_accounts.py
--rw-r--r--   0        0        0     3974 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/resources/webhooks.py
--rw-r--r--   0        0        0     8489 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/__init__.py
--rw-r--r--   0        0        0      871 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/account_detail.py
--rw-r--r--   0        0        0      556 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/account_detail_create_params.py
--rw-r--r--   0        0        0      305 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/account_detail_list_params.py
--rw-r--r--   0        0        0      689 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/connection.py
--rw-r--r--   0        0        0      475 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/connection_list_params.py
--rw-r--r--   0        0        0     4022 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/counterparty.py
--rw-r--r--   0        0        0     2154 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/counterparty_collect_account_params.py
--rw-r--r--   0        0        0      765 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/counterparty_collect_account_response.py
--rw-r--r--   0        0        0     4736 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/counterparty_create_params.py
--rw-r--r--   0        0        0      978 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/counterparty_list_params.py
--rw-r--r--   0        0        0      824 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/counterparty_update_params.py
--rw-r--r--   0        0        0     2016 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/document.py
--rw-r--r--   0        0        0      375 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/document_create_params.py
--rw-r--r--   0        0        0      295 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/document_list_params.py
--rw-r--r--   0        0        0      656 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/event.py
--rw-r--r--   0        0        0      527 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/event_list_params.py
--rw-r--r--   0        0        0     3367 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/expected_payment.py
--rw-r--r--   0        0        0     3583 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_create_params.py
--rw-r--r--   0        0        0     1619 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_list_params.py
--rw-r--r--   0        0        0      502 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_type.py
--rw-r--r--   0        0        0     2753 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_update_params.py
--rw-r--r--   0        0        0     2715 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/external_account.py
--rw-r--r--   0        0        0      309 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/external_account_complete_verification_params.py
--rw-r--r--   0        0        0     3247 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/external_account_create_params.py
--rw-r--r--   0        0        0      676 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/external_account_list_params.py
--rw-r--r--   0        0        0      235 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/external_account_type.py
--rw-r--r--   0        0        0     1424 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/external_account_update_params.py
--rw-r--r--   0        0        0     1054 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/external_account_verify_params.py
--rw-r--r--   0        0        0     2277 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail.py
--rw-r--r--   0        0        0     1052 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail_create_async_params.py
--rw-r--r--   0        0        0     1475 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail_list_params.py
--rw-r--r--   0        0        0      439 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail_update_params.py
--rw-r--r--   0        0        0     2365 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/internal_account.py
--rw-r--r--   0        0        0     1396 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/internal_account_create_params.py
--rw-r--r--   0        0        0     1210 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/internal_account_list_params.py
--rw-r--r--   0        0        0      656 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/internal_account_update_params.py
--rw-r--r--   0        0        0      249 2023-03-06 20:55:45.053854 modern_treasury-1.8.0/src/modern_treasury/types/internal_accounts/__init__.py
--rw-r--r--   0        0        0     2704 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/internal_accounts/balance_report.py
--rw-r--r--   0        0        0      592 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/internal_accounts/balance_report_list_params.py
--rw-r--r--   0        0        0      717 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger.py
--rw-r--r--   0        0        0     2787 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account.py
--rw-r--r--   0        0        0     2802 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category.py
--rw-r--r--   0        0        0     1007 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_create_params.py
--rw-r--r--   0        0        0      706 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_list_params.py
--rw-r--r--   0        0        0      632 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_retrieve_params.py
--rw-r--r--   0        0        0      573 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_update_params.py
--rw-r--r--   0        0        0      937 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_create_params.py
--rw-r--r--   0        0        0     1265 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_list_params.py
--rw-r--r--   0        0        0     1845 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout.py
--rw-r--r--   0        0        0     1340 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout_create_params.py
--rw-r--r--   0        0        0      352 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout_list_params.py
--rw-r--r--   0        0        0      685 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout_update_params.py
--rw-r--r--   0        0        0      593 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_retrieve_params.py
--rw-r--r--   0        0        0      648 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_update_params.py
--rw-r--r--   0        0        0      550 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_create_params.py
--rw-r--r--   0        0        0     4120 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_entry.py
--rw-r--r--   0        0        0     2101 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_entry_list_params.py
--rw-r--r--   0        0        0      783 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_list_params.py
--rw-r--r--   0        0        0     2442 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction.py
--rw-r--r--   0        0        0     4044 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction_create_params.py
--rw-r--r--   0        0        0     1723 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction_list_params.py
--rw-r--r--   0        0        0     2990 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction_update_params.py
--rw-r--r--   0        0        0      348 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/__init__.py
--rw-r--r--   0        0        0     7847 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/ledger_transaction_version.py
--rw-r--r--   0        0        0      759 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/version_list_params.py
--rw-r--r--   0        0        0      767 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/version_versions_params.py
--rw-r--r--   0        0        0      530 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ledger_update_params.py
--rw-r--r--   0        0        0     2038 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/line_item.py
--rw-r--r--   0        0        0      295 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/line_item_list_params.py
--rw-r--r--   0        0        0      381 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/line_item_update_params.py
--rw-r--r--   0        0        0     1672 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/paper_item.py
--rw-r--r--   0        0        0      680 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/paper_item_list_params.py
--rw-r--r--   0        0        0    10864 2023-03-06 20:55:45.553854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order.py
--rw-r--r--   0        0        0    16331 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order_create_async_params.py
--rw-r--r--   0        0        0    16872 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order_create_params.py
--rw-r--r--   0        0        0     1868 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order_list_params.py
--rw-r--r--   0        0        0      245 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order_subtype.py
--rw-r--r--   0        0        0      380 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order_type.py
--rw-r--r--   0        0        0    13102 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_order_update_params.py
--rw-r--r--   0        0        0      289 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/payment_orders/__init__.py
--rw-r--r--   0        0        0     1033 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_orders/reversal.py
--rw-r--r--   0        0        0     5102 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_orders/reversal_create_params.py
--rw-r--r--   0        0        0      295 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/payment_orders/reversal_list_params.py
--rw-r--r--   0        0        0     2533 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/payment_reference.py
--rw-r--r--   0        0        0      773 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/payment_reference_list_params.py
--rw-r--r--   0        0        0      161 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/ping_response.py
--rw-r--r--   0        0        0     1995 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/return_create_params.py
--rw-r--r--   0        0        0      942 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/return_list_params.py
--rw-r--r--   0        0        0     5795 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/return_object.py
--rw-r--r--   0        0        0     2040 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/routing_detail.py
--rw-r--r--   0        0        0     1160 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/routing_detail_create_params.py
--rw-r--r--   0        0        0      305 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/routing_detail_list_params.py
--rw-r--r--   0        0        0     2194 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/routing_number_lookup_request.py
--rw-r--r--   0        0        0      212 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared/__init__.py
--rw-r--r--   0        0        0      222 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared/accounts_type.py
--rw-r--r--   0        0        0      215 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared/async_response.py
--rw-r--r--   0        0        0     3058 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared/currency.py
--rw-r--r--   0        0        0      212 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared_params/__init__.py
--rw-r--r--   0        0        0      222 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared_params/accounts_type.py
--rw-r--r--   0        0        0      265 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared_params/async_response.py
--rw-r--r--   0        0        0     3058 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/shared_params/currency.py
--rw-r--r--   0        0        0     3947 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/transaction.py
--rw-r--r--   0        0        0     1258 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/transaction_list_params.py
--rw-r--r--   0        0        0      419 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/transaction_update_params.py
--rw-r--r--   0        0        0      792 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/validation_validate_routing_number_params.py
--rw-r--r--   0        0        0     1791 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/virtual_account.py
--rw-r--r--   0        0        0     4942 2023-03-06 20:55:45.563854 modern_treasury-1.8.0/src/modern_treasury/types/virtual_account_create_params.py
--rw-r--r--   0        0        0      597 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/virtual_account_list_params.py
--rw-r--r--   0        0        0      346 2023-03-06 20:55:45.063854 modern_treasury-1.8.0/src/modern_treasury/types/virtual_account_update_params.py
--rw-r--r--   0        0        0    17688 1970-01-01 00:00:00.000000 modern_treasury-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/LICENSE
+-rw-r--r--   0        0        0    17913 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/README.md
+-rw-r--r--   0        0        0     1644 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1781 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/__init__.py
+-rw-r--r--   0        0        0    36088 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_base_exceptions.py
+-rw-r--r--   0        0        0    19928 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_client.py
+-rw-r--r--   0        0        0      723 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_exceptions.py
+-rw-r--r--   0        0        0     7120 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_models.py
+-rw-r--r--   0        0        0     4781 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_qs.py
+-rw-r--r--   0        0        0      926 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_resource.py
+-rw-r--r--   0        0        0     3961 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_types.py
+-rw-r--r--   0        0        0     1224 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_utils/__init__.py
+-rw-r--r--   0        0        0     6701 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_utils/_transform.py
+-rw-r--r--   0        0        0     9210 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_utils/_utils.py
+-rw-r--r--   0        0        0      106 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/_version.py
+-rw-r--r--   0        0        0     2010 2023-03-08 19:20:02.067736 modern_treasury-1.9.0/src/modern_treasury/pagination.py
+-rw-r--r--   0        0        0        0 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/py.typed
+-rw-r--r--   0        0        0     2864 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/__init__.py
+-rw-r--r--   0        0        0    10955 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/account_details.py
+-rw-r--r--   0        0        0     4138 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/connections.py
+-rw-r--r--   0        0        0    25757 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/counterparties.py
+-rw-r--r--   0        0        0    10607 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/documents.py
+-rw-r--r--   0        0        0     6098 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/events.py
+-rw-r--r--   0        0        0    29200 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/expected_payments.py
+-rw-r--r--   0        0        0    26166 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/external_accounts.py
+-rw-r--r--   0        0        0    16818 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/incoming_payment_details.py
+-rw-r--r--   0        0        0      288 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/internal_accounts/__init__.py
+-rw-r--r--   0        0        0     6431 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/internal_accounts/balance_reports.py
+-rw-r--r--   0        0        0    16975 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/internal_accounts/internal_accounts.py
+-rw-r--r--   0        0        0    25469 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_account_categories.py
+-rw-r--r--   0        0        0    14662 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_account_payouts.py
+-rw-r--r--   0        0        0    19352 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_accounts.py
+-rw-r--r--   0        0        0    10797 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_entries.py
+-rw-r--r--   0        0        0      267 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_transactions/__init__.py
+-rw-r--r--   0        0        0    21086 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_transactions/ledger_transactions.py
+-rw-r--r--   0        0        0     8707 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledger_transactions/versions.py
+-rw-r--r--   0        0        0    13900 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/ledgers.py
+-rw-r--r--   0        0        0     8076 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/line_items.py
+-rw-r--r--   0        0        0     6343 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/paper_items.py
+-rw-r--r--   0        0        0      247 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/payment_orders/__init__.py
+-rw-r--r--   0        0        0    85851 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/payment_orders/payment_orders.py
+-rw-r--r--   0        0        0     9828 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/payment_orders/reversals.py
+-rw-r--r--   0        0        0     6597 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/payment_references.py
+-rw-r--r--   0        0        0    14013 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/returns.py
+-rw-r--r--   0        0        0    12417 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/routing_details.py
+-rw-r--r--   0        0        0    11477 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/transactions.py
+-rw-r--r--   0        0        0     4566 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/validations.py
+-rw-r--r--   0        0        0    16878 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/virtual_accounts.py
+-rw-r--r--   0        0        0     3974 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/resources/webhooks.py
+-rw-r--r--   0        0        0     8489 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/__init__.py
+-rw-r--r--   0        0        0      916 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/account_detail.py
+-rw-r--r--   0        0        0      556 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/account_detail_create_params.py
+-rw-r--r--   0        0        0      305 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/account_detail_list_params.py
+-rw-r--r--   0        0        0      734 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/connection.py
+-rw-r--r--   0        0        0      475 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/connection_list_params.py
+-rw-r--r--   0        0        0     4107 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/counterparty.py
+-rw-r--r--   0        0        0     2154 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/counterparty_collect_account_params.py
+-rw-r--r--   0        0        0      765 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/counterparty_collect_account_response.py
+-rw-r--r--   0        0        0     4736 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/counterparty_create_params.py
+-rw-r--r--   0        0        0     1181 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/counterparty_list_params.py
+-rw-r--r--   0        0        0      824 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/counterparty_update_params.py
+-rw-r--r--   0        0        0     2076 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/document.py
+-rw-r--r--   0        0        0      375 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/document_create_params.py
+-rw-r--r--   0        0        0      295 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/document_list_params.py
+-rw-r--r--   0        0        0      702 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/event.py
+-rw-r--r--   0        0        0      730 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/event_list_params.py
+-rw-r--r--   0        0        0     3415 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/expected_payment.py
+-rw-r--r--   0        0        0     3773 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_create_params.py
+-rw-r--r--   0        0        0     1822 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_list_params.py
+-rw-r--r--   0        0        0      502 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_type.py
+-rw-r--r--   0        0        0     2943 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_update_params.py
+-rw-r--r--   0        0        0     2785 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account.py
+-rw-r--r--   0        0        0      309 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account_complete_verification_params.py
+-rw-r--r--   0        0        0     3247 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account_create_params.py
+-rw-r--r--   0        0        0      676 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account_list_params.py
+-rw-r--r--   0        0        0      235 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account_type.py
+-rw-r--r--   0        0        0     1424 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account_update_params.py
+-rw-r--r--   0        0        0     1054 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/external_account_verify_params.py
+-rw-r--r--   0        0        0     2324 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail.py
+-rw-r--r--   0        0        0     1186 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail_create_async_params.py
+-rw-r--r--   0        0        0     1666 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail_list_params.py
+-rw-r--r--   0        0        0      439 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail_update_params.py
+-rw-r--r--   0        0        0     2415 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_account.py
+-rw-r--r--   0        0        0     1396 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_account_create_params.py
+-rw-r--r--   0        0        0     1210 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_account_list_params.py
+-rw-r--r--   0        0        0      656 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_account_update_params.py
+-rw-r--r--   0        0        0      249 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_accounts/__init__.py
+-rw-r--r--   0        0        0     2761 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_accounts/balance_report.py
+-rw-r--r--   0        0        0      728 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/internal_accounts/balance_report_list_params.py
+-rw-r--r--   0        0        0      762 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger.py
+-rw-r--r--   0        0        0     2832 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account.py
+-rw-r--r--   0        0        0     2847 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category.py
+-rw-r--r--   0        0        0     1007 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_create_params.py
+-rw-r--r--   0        0        0      706 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_list_params.py
+-rw-r--r--   0        0        0      855 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_retrieve_params.py
+-rw-r--r--   0        0        0      573 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_update_params.py
+-rw-r--r--   0        0        0      937 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_create_params.py
+-rw-r--r--   0        0        0     1487 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_list_params.py
+-rw-r--r--   0        0        0     1885 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout.py
+-rw-r--r--   0        0        0     1340 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout_create_params.py
+-rw-r--r--   0        0        0      352 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout_list_params.py
+-rw-r--r--   0        0        0      685 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout_update_params.py
+-rw-r--r--   0        0        0      746 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_retrieve_params.py
+-rw-r--r--   0        0        0      648 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_update_params.py
+-rw-r--r--   0        0        0      550 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_create_params.py
+-rw-r--r--   0        0        0     4165 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_entry.py
+-rw-r--r--   0        0        0     2174 2023-03-08 19:20:02.077737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_entry_list_params.py
+-rw-r--r--   0        0        0      837 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_list_params.py
+-rw-r--r--   0        0        0     2490 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction.py
+-rw-r--r--   0        0        0     4179 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction_create_params.py
+-rw-r--r--   0        0        0     1811 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction_list_params.py
+-rw-r--r--   0        0        0     2990 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction_update_params.py
+-rw-r--r--   0        0        0      348 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/__init__.py
+-rw-r--r--   0        0        0     7894 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/ledger_transaction_version.py
+-rw-r--r--   0        0        0      813 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/version_list_params.py
+-rw-r--r--   0        0        0      821 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/version_versions_params.py
+-rw-r--r--   0        0        0      530 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ledger_update_params.py
+-rw-r--r--   0        0        0     2078 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/line_item.py
+-rw-r--r--   0        0        0      295 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/line_item_list_params.py
+-rw-r--r--   0        0        0      381 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/line_item_update_params.py
+-rw-r--r--   0        0        0     1719 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/paper_item.py
+-rw-r--r--   0        0        0      871 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/paper_item_list_params.py
+-rw-r--r--   0        0        0    10926 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order.py
+-rw-r--r--   0        0        0    16591 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order_create_async_params.py
+-rw-r--r--   0        0        0    17132 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order_create_params.py
+-rw-r--r--   0        0        0     2059 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order_list_params.py
+-rw-r--r--   0        0        0      245 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order_subtype.py
+-rw-r--r--   0        0        0      380 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order_type.py
+-rw-r--r--   0        0        0    13306 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_order_update_params.py
+-rw-r--r--   0        0        0      289 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_orders/__init__.py
+-rw-r--r--   0        0        0     1073 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_orders/reversal.py
+-rw-r--r--   0        0        0     5238 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_orders/reversal_create_params.py
+-rw-r--r--   0        0        0      295 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_orders/reversal_list_params.py
+-rw-r--r--   0        0        0     2573 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_reference.py
+-rw-r--r--   0        0        0      773 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/payment_reference_list_params.py
+-rw-r--r--   0        0        0      161 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/ping_response.py
+-rw-r--r--   0        0        0     2130 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/return_create_params.py
+-rw-r--r--   0        0        0      942 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/return_list_params.py
+-rw-r--r--   0        0        0     5852 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/return_object.py
+-rw-r--r--   0        0        0     2095 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/routing_detail.py
+-rw-r--r--   0        0        0     1160 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/routing_detail_create_params.py
+-rw-r--r--   0        0        0      305 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/routing_detail_list_params.py
+-rw-r--r--   0        0        0     2194 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/routing_number_lookup_request.py
+-rw-r--r--   0        0        0      212 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared/__init__.py
+-rw-r--r--   0        0        0      222 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared/accounts_type.py
+-rw-r--r--   0        0        0      215 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared/async_response.py
+-rw-r--r--   0        0        0     3058 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared/currency.py
+-rw-r--r--   0        0        0      212 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      222 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared_params/accounts_type.py
+-rw-r--r--   0        0        0      265 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared_params/async_response.py
+-rw-r--r--   0        0        0     3058 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/shared_params/currency.py
+-rw-r--r--   0        0        0     3999 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/transaction.py
+-rw-r--r--   0        0        0     1449 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/transaction_list_params.py
+-rw-r--r--   0        0        0      419 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/transaction_update_params.py
+-rw-r--r--   0        0        0      792 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/validation_validate_routing_number_params.py
+-rw-r--r--   0        0        0     1836 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/virtual_account.py
+-rw-r--r--   0        0        0     5505 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/virtual_account_create_params.py
+-rw-r--r--   0        0        0      597 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/virtual_account_list_params.py
+-rw-r--r--   0        0        0      346 2023-03-08 19:20:02.087737 modern_treasury-1.9.0/src/modern_treasury/types/virtual_account_update_params.py
+-rw-r--r--   0        0        0    18852 1970-01-01 00:00:00.000000 modern_treasury-1.9.0/PKG-INFO
```

### Comparing `modern_treasury-1.8.0/LICENSE` & `modern_treasury-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/README.md` & `modern_treasury-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: modern-treasury
+Version: 1.9.0
+Summary: Client library for the Modern Treasury API
+Home-page: https://github.com/Modern-Treasury/modern-treasury-python
+License: MIT
+Author: Modern Treasury
+Author-email: sdk-feedback@moderntreasury.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anyio (>=3.5.0)
+Requires-Dist: distro (>=1.7.0)
+Requires-Dist: httpx (>=0.23.0)
+Requires-Dist: pydantic (>=1.9.0)
+Requires-Dist: typing-extensions (>=4.1.1)
+Project-URL: Repository, https://github.com/Modern-Treasury/modern-treasury-python
+Description-Content-Type: text/markdown
+
 # Modern Treasury Python API Library
 
 > **Migration Guide**
 >
 > We've made some major improvements to how you pass arguments to methods which will require migrating your existing code.
 >
 > If you want to migrate to the new patterns incrementally you can do so by installing `v0.5.0`. This release contains both
@@ -521,18 +545,52 @@
 - `ReceivingAccountContactDetails` -> `ReceivingAccountContactDetail`
 - `ReceivingAccountRoutingDetails` -> `ReceivingAccountRoutingDetail`
 - `LedgerEntriesResultingLedgerAccountBalances` -> `LedgerEntryResultingLedgerAccountBalances`
 - `LedgerEntriesResultingLedgerAccountBalancesPostedBalance` -> `LedgerEntryResultingLedgerAccountBalancesPostedBalance`
 - `LedgerEntriesResultingLedgerAccountBalancesPendingBalance` -> `LedgerEntryResultingLedgerAccountBalancesPendingBalance`
 - `LedgerEntriesResultingLedgerAccountBalancesAvailableBalance` -> `LedgerEntryResultingLedgerAccountBalancesAvailableBalance`
 
+## Rich `date` and `datetime` types
+
+We've improved the types for response fields / request params that correspond to `date` or `datetime` values!
+
+Previously they were just raw strings but now response fields will be instances of `date` or `datetime`.
+
+This means that if you're working with these fields and parsing them into `datetime` instances manually you will have to remove
+any code that performs said parsing.
+
+```diff
+account = client.internal_accounts.retrieve('<id>')
+- created_at = datetime.fromisoformat(account.created_at)
++ created_at = account.created_at
+print(created_at.month)
+```
+
+For request params you can continue to pass in strings if you want to use a datetime library other than the standard library version but if you
+were writing code that looked like this:
+
+```py
+dt = datetime(...)
+for counterparty in client.counterparties.list(created_at_upper_bound=dt.isoformat()):
+  ...
+```
+
+You can remove the explicit call to `isoformat`!
+
+```diff
+dt = datetime(...)
+- for counterparty in client.counterparties.list(created_at_upper_bound=dt.isoformat()):
++ for counterparty in client.counterparties.list(created_at_upper_bound=dt):
+  ...
+```
+
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please email us at [sdk-feedback@moderntreasury.com](mailto:sdk-feedback@moderntreasury.com) or open an issue with questions,
 bugs, or suggestions.
 
 ## Requirements
 
-Python 3.7 or higher.
+Python 3.7 or higher.
```

### Comparing `modern_treasury-1.8.0/pyproject.toml` & `modern_treasury-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modern-treasury"
-version = "1.8.0"
+version = "1.9.0"
 description = "Client library for the Modern Treasury API"
 readme = "README.md"
 authors = ["Modern Treasury <sdk-feedback@moderntreasury.com>"]
 license = "MIT"
 repository = "https://github.com/Modern-Treasury/modern-treasury-python"
 packages = [
   { include = "modern_treasury", from = "src" }
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/__init__.py` & `modern_treasury-1.9.0/src/modern_treasury/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_base_client.py` & `modern_treasury-1.9.0/src/modern_treasury/_base_client.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_base_exceptions.py` & `modern_treasury-1.9.0/src/modern_treasury/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_client.py` & `modern_treasury-1.9.0/src/modern_treasury/_client.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_exceptions.py` & `modern_treasury-1.9.0/src/modern_treasury/_exceptions.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_models.py` & `modern_treasury-1.9.0/src/modern_treasury/_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 from typing import Any, Type, Union, cast
+from datetime import date, datetime
 from typing_extensions import final
 
 import pydantic
 import pydantic.generics
 from pydantic.fields import ModelField
 from pydantic.typing import (
     get_args,
     is_union,
     get_origin,
     is_none_type,
     is_literal_type,
 )
+from pydantic.datetime_parse import parse_date
 
 from ._types import (
     Body,
     Query,
     ModelT,
     Headers,
     Timeout,
     NotGiven,
     AnyMapping,
     RequestFiles,
 )
-from ._utils import is_list, is_mapping, strip_not_given
+from ._utils import is_list, is_mapping, parse_datetime, strip_not_given
 
 __all__ = ["BaseModel", "GenericModel"]
 
 
 class BaseModel(pydantic.BaseModel):
     def __str__(self) -> str:
         return f'{self.__repr_name__()}({self.__repr_str__(", ")})'
@@ -130,14 +132,26 @@
 
     if origin == int:
         try:
             return int(value)  # type: ignore
         except Exception:
             return value
 
+    if type_ == datetime:
+        try:
+            return parse_datetime(value)  # type: ignore
+        except Exception:
+            return value
+
+    if type_ == date:
+        try:
+            return parse_date(value)  # type: ignore
+        except Exception:
+            return value
+
     if not is_literal_type(type_) and (issubclass(origin, BaseModel) or issubclass(origin, GenericModel)):
         if is_list(value):
             return [cast(Any, type_).construct(**entry) if is_mapping(entry) else entry for entry in value]
 
         if is_mapping(value):
             if issubclass(type_, BaseModel):
                 return type_.construct(**value)  # type: ignore[arg-type]
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_qs.py` & `modern_treasury-1.9.0/src/modern_treasury/_qs.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_resource.py` & `modern_treasury-1.9.0/src/modern_treasury/_resource.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_types.py` & `modern_treasury-1.9.0/src/modern_treasury/_types.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_utils/__init__.py` & `modern_treasury-1.9.0/src/modern_treasury/_utils/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from ._utils import flatten as flatten
 from ._utils import is_dict as is_dict
 from ._utils import is_list as is_list
 from ._utils import is_mapping as is_mapping
+from ._utils import parse_date as parse_date
 from ._utils import coerce_float as coerce_float
 from ._utils import is_list_type as is_list_type
 from ._utils import removeprefix as removeprefix
 from ._utils import removesuffix as removesuffix
 from ._utils import extract_files as extract_files
 from ._utils import is_union_type as is_union_type
 from ._utils import required_args as required_args
 from ._utils import coerce_boolean as coerce_boolean
 from ._utils import coerce_integer as coerce_integer
+from ._utils import parse_datetime as parse_datetime
 from ._utils import strip_not_given as strip_not_given
 from ._utils import deepcopy_minimal as deepcopy_minimal
 from ._utils import extract_type_arg as extract_type_arg
 from ._utils import is_required_type as is_required_type
 from ._utils import is_annotated_type as is_annotated_type
 from ._utils import strip_annotated_type as strip_annotated_type
 from ._transform import PropertyInfo as PropertyInfo
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/_utils/_utils.py` & `modern_treasury-1.9.0/src/modern_treasury/_utils/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import inspect
 import functools
 from typing import Any, Mapping, TypeVar, Callable, Iterable, Sequence, cast, overload
 from typing_extensions import Required, Annotated, TypeGuard, get_args, get_origin
 
 from pydantic.typing import is_union as _is_union
 
+# re-export for forwards compat
+from pydantic.datetime_parse import parse_date as parse_date
+from pydantic.datetime_parse import parse_datetime as parse_datetime
+
 from .._types import NotGiven, FileTypes
 
 _T = TypeVar("_T")
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
 
 
 def flatten(t: Iterable[Iterable[_T]]) -> list[_T]:
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/pagination.py` & `modern_treasury-1.9.0/src/modern_treasury/pagination.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/__init__.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/account_details.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/account_details.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Optional
 from typing_extensions import Literal
 
-from ..types import AccountDetail
+from ..types import (
+    AccountDetail,
+    account_detail_list_params,
+    account_detail_create_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["AccountDetails", "AsyncAccountDetails"]
 
 
@@ -41,18 +46,21 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             f"/api/{accounts_type}/{account_id}/account_details",
-            body={
-                "account_number": account_number,
-                "account_number_type": account_number_type,
-            },
+            body=maybe_transform(
+                {
+                    "account_number": account_number,
+                    "account_number_type": account_number_type,
+                },
+                account_detail_create_params.AccountDetailCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=AccountDetail,
         )
 
     def retrieve(
         self,
         id: str,
@@ -98,18 +106,21 @@
         return self._get_api_list(
             f"/api/{accounts_type}/{account_id}/account_details",
             page=SyncPage[AccountDetail],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    account_detail_list_params.AccountDetailListParams,
+                ),
             ),
             model=AccountDetail,
         )
 
     def delete(
         self,
         id: str,
@@ -158,18 +169,21 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             f"/api/{accounts_type}/{account_id}/account_details",
-            body={
-                "account_number": account_number,
-                "account_number_type": account_number_type,
-            },
+            body=maybe_transform(
+                {
+                    "account_number": account_number,
+                    "account_number_type": account_number_type,
+                },
+                account_detail_create_params.AccountDetailCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=AccountDetail,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -215,18 +229,21 @@
         return self._get_api_list(
             f"/api/{accounts_type}/{account_id}/account_details",
             page=AsyncPage[AccountDetail],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    account_detail_list_params.AccountDetailListParams,
+                ),
             ),
             model=AccountDetail,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/connections.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/connections.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Optional
 
-from ..types import Connection
+from ..types import Connection, connection_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Connections", "AsyncConnections"]
 
 
@@ -44,20 +45,23 @@
         return self._get_api_list(
             "/api/connections",
             page=SyncPage[Connection],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "vendor_customer_id": vendor_customer_id,
-                    "entity": entity,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "vendor_customer_id": vendor_customer_id,
+                        "entity": entity,
+                    },
+                    connection_list_params.ConnectionListParams,
+                ),
             ),
             model=Connection,
         )
 
 
 class AsyncConnections(AsyncAPIResource):
     def list(
@@ -90,16 +94,19 @@
         return self._get_api_list(
             "/api/connections",
             page=AsyncPage[Connection],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "vendor_customer_id": vendor_customer_id,
-                    "entity": entity,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "vendor_customer_id": vendor_customer_id,
+                        "entity": entity,
+                    },
+                    connection_list_params.ConnectionListParams,
+                ),
             ),
             model=Connection,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/counterparties.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/counterparties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
+from typing import Dict, List, Union, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from ..types import (
     Counterparty,
     CounterpartyCollectAccountResponse,
+    counterparty_list_params,
     counterparty_create_params,
+    counterparty_update_params,
+    counterparty_collect_account_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Counterparties", "AsyncCounterparties"]
 
 
@@ -61,24 +66,27 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/counterparties",
-            body={
-                "name": name,
-                "accounts": accounts,
-                "email": email,
-                "metadata": metadata,
-                "send_remittance_advice": send_remittance_advice,
-                "accounting": accounting,
-                "ledger_type": ledger_type,
-                "taxpayer_identifier": taxpayer_identifier,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "accounts": accounts,
+                    "email": email,
+                    "metadata": metadata,
+                    "send_remittance_advice": send_remittance_advice,
+                    "accounting": accounting,
+                    "ledger_type": ledger_type,
+                    "taxpayer_identifier": taxpayer_identifier,
+                },
+                counterparty_create_params.CounterpartyCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Counterparty,
         )
 
     def retrieve(
         self,
         id: str,
@@ -131,35 +139,38 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/counterparties/{id}",
-            body={
-                "name": name,
-                "email": email,
-                "metadata": metadata,
-                "send_remittance_advice": send_remittance_advice,
-                "taxpayer_identifier": taxpayer_identifier,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "email": email,
+                    "metadata": metadata,
+                    "send_remittance_advice": send_remittance_advice,
+                    "taxpayer_identifier": taxpayer_identifier,
+                },
+                counterparty_update_params.CounterpartyUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Counterparty,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         name: str | NotGiven = NOT_GIVEN,
         email: str | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        created_at_lower_bound: str | NotGiven = NOT_GIVEN,
-        created_at_upper_bound: str | NotGiven = NOT_GIVEN,
+        created_at_lower_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
+        created_at_upper_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[Counterparty]:
         """
@@ -189,23 +200,26 @@
         return self._get_api_list(
             "/api/counterparties",
             page=SyncPage[Counterparty],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "name": name,
-                    "email": email,
-                    "metadata": metadata,
-                    "created_at_lower_bound": created_at_lower_bound,
-                    "created_at_upper_bound": created_at_upper_bound,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "name": name,
+                        "email": email,
+                        "metadata": metadata,
+                        "created_at_lower_bound": created_at_lower_bound,
+                        "created_at_upper_bound": created_at_upper_bound,
+                    },
+                    counterparty_list_params.CounterpartyListParams,
+                ),
             ),
             model=Counterparty,
         )
 
     def delete(
         self,
         id: str,
@@ -290,20 +304,23 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             f"/api/counterparties/{id}/collect_account",
-            body={
-                "direction": direction,
-                "send_email": send_email,
-                "fields": fields,
-                "custom_redirect": custom_redirect,
-            },
+            body=maybe_transform(
+                {
+                    "direction": direction,
+                    "send_email": send_email,
+                    "fields": fields,
+                    "custom_redirect": custom_redirect,
+                },
+                counterparty_collect_account_params.CounterpartyCollectAccountParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=CounterpartyCollectAccountResponse,
         )
 
 
 class AsyncCounterparties(AsyncAPIResource):
     async def create(
@@ -348,24 +365,27 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/counterparties",
-            body={
-                "name": name,
-                "accounts": accounts,
-                "email": email,
-                "metadata": metadata,
-                "send_remittance_advice": send_remittance_advice,
-                "accounting": accounting,
-                "ledger_type": ledger_type,
-                "taxpayer_identifier": taxpayer_identifier,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "accounts": accounts,
+                    "email": email,
+                    "metadata": metadata,
+                    "send_remittance_advice": send_remittance_advice,
+                    "accounting": accounting,
+                    "ledger_type": ledger_type,
+                    "taxpayer_identifier": taxpayer_identifier,
+                },
+                counterparty_create_params.CounterpartyCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Counterparty,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -418,35 +438,38 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/counterparties/{id}",
-            body={
-                "name": name,
-                "email": email,
-                "metadata": metadata,
-                "send_remittance_advice": send_remittance_advice,
-                "taxpayer_identifier": taxpayer_identifier,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "email": email,
+                    "metadata": metadata,
+                    "send_remittance_advice": send_remittance_advice,
+                    "taxpayer_identifier": taxpayer_identifier,
+                },
+                counterparty_update_params.CounterpartyUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Counterparty,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         name: str | NotGiven = NOT_GIVEN,
         email: str | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        created_at_lower_bound: str | NotGiven = NOT_GIVEN,
-        created_at_upper_bound: str | NotGiven = NOT_GIVEN,
+        created_at_lower_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
+        created_at_upper_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[Counterparty, AsyncPage[Counterparty]]:
         """
@@ -476,23 +499,26 @@
         return self._get_api_list(
             "/api/counterparties",
             page=AsyncPage[Counterparty],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "name": name,
-                    "email": email,
-                    "metadata": metadata,
-                    "created_at_lower_bound": created_at_lower_bound,
-                    "created_at_upper_bound": created_at_upper_bound,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "name": name,
+                        "email": email,
+                        "metadata": metadata,
+                        "created_at_lower_bound": created_at_lower_bound,
+                        "created_at_upper_bound": created_at_upper_bound,
+                    },
+                    counterparty_list_params.CounterpartyListParams,
+                ),
             ),
             model=Counterparty,
         )
 
     async def delete(
         self,
         id: str,
@@ -577,16 +603,19 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             f"/api/counterparties/{id}/collect_account",
-            body={
-                "direction": direction,
-                "send_email": send_email,
-                "fields": fields,
-                "custom_redirect": custom_redirect,
-            },
+            body=maybe_transform(
+                {
+                    "direction": direction,
+                    "send_email": send_email,
+                    "fields": fields,
+                    "custom_redirect": custom_redirect,
+                },
+                counterparty_collect_account_params.CounterpartyCollectAccountParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=CounterpartyCollectAccountResponse,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/documents.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/documents.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Mapping, Optional, cast
 from typing_extensions import Literal
 
-from ..types import Document
+from ..types import Document, document_list_params, document_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven, FileTypes
-from .._utils import extract_files, deepcopy_minimal
+from .._utils import extract_files, maybe_transform, deepcopy_minimal
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Documents", "AsyncDocuments"]
 
 
@@ -62,15 +62,15 @@
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
 
         return self._post(
             f"/api/{documentable_type}/{documentable_id}/documents",
-            body=body,
+            body=maybe_transform(body, document_create_params.DocumentCreateParams),
             files=files,
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Document,
         )
 
     def retrieve(
         self,
@@ -137,18 +137,21 @@
         return self._get_api_list(
             f"/api/{documentable_type}/{documentable_id}/documents",
             page=SyncPage[Document],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    document_list_params.DocumentListParams,
+                ),
             ),
             model=Document,
         )
 
 
 class AsyncDocuments(AsyncAPIResource):
     async def create(
@@ -197,15 +200,15 @@
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
 
         return await self._post(
             f"/api/{documentable_type}/{documentable_id}/documents",
-            body=body,
+            body=maybe_transform(body, document_create_params.DocumentCreateParams),
             files=files,
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Document,
         )
 
     async def retrieve(
         self,
@@ -272,14 +275,17 @@
         return self._get_api_list(
             f"/api/{documentable_type}/{documentable_id}/documents",
             page=AsyncPage[Document],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    document_list_params.DocumentListParams,
+                ),
             ),
             model=Document,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/events.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Union, Optional
+from datetime import datetime
 
-from ..types import Event
+from ..types import Event, event_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Events", "AsyncEvents"]
 
 
@@ -32,16 +34,16 @@
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
-        event_time_start: str | NotGiven = NOT_GIVEN,
-        event_time_end: str | NotGiven = NOT_GIVEN,
+        event_time_start: Union[str, datetime] | NotGiven = NOT_GIVEN,
+        event_time_end: Union[str, datetime] | NotGiven = NOT_GIVEN,
         resource: str | NotGiven = NOT_GIVEN,
         entity_id: str | NotGiven = NOT_GIVEN,
         event_name: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -64,23 +66,26 @@
         return self._get_api_list(
             "/api/events",
             page=SyncPage[Event],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "event_time_start": event_time_start,
-                    "event_time_end": event_time_end,
-                    "resource": resource,
-                    "entity_id": entity_id,
-                    "event_name": event_name,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "event_time_start": event_time_start,
+                        "event_time_end": event_time_end,
+                        "resource": resource,
+                        "entity_id": entity_id,
+                        "event_name": event_name,
+                    },
+                    event_list_params.EventListParams,
+                ),
             ),
             model=Event,
         )
 
 
 class AsyncEvents(AsyncAPIResource):
     async def retrieve(
@@ -101,16 +106,16 @@
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
-        event_time_start: str | NotGiven = NOT_GIVEN,
-        event_time_end: str | NotGiven = NOT_GIVEN,
+        event_time_start: Union[str, datetime] | NotGiven = NOT_GIVEN,
+        event_time_end: Union[str, datetime] | NotGiven = NOT_GIVEN,
         resource: str | NotGiven = NOT_GIVEN,
         entity_id: str | NotGiven = NOT_GIVEN,
         event_name: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -133,19 +138,22 @@
         return self._get_api_list(
             "/api/events",
             page=AsyncPage[Event],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "event_time_start": event_time_start,
-                    "event_time_end": event_time_end,
-                    "resource": resource,
-                    "entity_id": entity_id,
-                    "event_name": event_name,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "event_time_start": event_time_start,
+                        "event_time_end": event_time_end,
+                        "resource": resource,
+                        "entity_id": entity_id,
+                        "event_name": event_name,
+                    },
+                    event_list_params.EventListParams,
+                ),
             ),
             model=Event,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/expected_payments.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/expected_payments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
+from typing import Dict, List, Union, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import (
     ExpectedPayment,
     ExpectedPaymentType,
     shared_params,
+    expected_payment_list_params,
     expected_payment_create_params,
+    expected_payment_update_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["ExpectedPayments", "AsyncExpectedPayments"]
 
 
@@ -25,16 +29,16 @@
         *,
         amount_upper_bound: int,
         amount_lower_bound: int,
         direction: Literal["credit", "debit"],
         internal_account_id: str,
         type: ExpectedPaymentType | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        date_upper_bound: Optional[str] | NotGiven = NOT_GIVEN,
-        date_lower_bound: Optional[str] | NotGiven = NOT_GIVEN,
+        date_upper_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
+        date_lower_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         counterparty_id: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         line_items: List[expected_payment_create_params.LineItem] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -87,30 +91,33 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/expected_payments",
-            body={
-                "amount_upper_bound": amount_upper_bound,
-                "amount_lower_bound": amount_lower_bound,
-                "direction": direction,
-                "internal_account_id": internal_account_id,
-                "type": type,
-                "currency": currency,
-                "date_upper_bound": date_upper_bound,
-                "date_lower_bound": date_lower_bound,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "metadata": metadata,
-                "counterparty_id": counterparty_id,
-                "remittance_information": remittance_information,
-                "line_items": line_items,
-            },
+            body=maybe_transform(
+                {
+                    "amount_upper_bound": amount_upper_bound,
+                    "amount_lower_bound": amount_lower_bound,
+                    "direction": direction,
+                    "internal_account_id": internal_account_id,
+                    "type": type,
+                    "currency": currency,
+                    "date_upper_bound": date_upper_bound,
+                    "date_lower_bound": date_lower_bound,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "metadata": metadata,
+                    "counterparty_id": counterparty_id,
+                    "remittance_information": remittance_information,
+                    "line_items": line_items,
+                },
+                expected_payment_create_params.ExpectedPaymentCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExpectedPayment,
         )
 
     def retrieve(
         self,
         id: str,
@@ -134,16 +141,16 @@
         *,
         amount_upper_bound: int | NotGiven = NOT_GIVEN,
         amount_lower_bound: int | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         internal_account_id: str | NotGiven = NOT_GIVEN,
         type: ExpectedPaymentType | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        date_upper_bound: Optional[str] | NotGiven = NOT_GIVEN,
-        date_lower_bound: Optional[str] | NotGiven = NOT_GIVEN,
+        date_upper_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
+        date_lower_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         counterparty_id: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -195,29 +202,32 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/expected_payments/{id}",
-            body={
-                "amount_upper_bound": amount_upper_bound,
-                "amount_lower_bound": amount_lower_bound,
-                "direction": direction,
-                "internal_account_id": internal_account_id,
-                "type": type,
-                "currency": currency,
-                "date_upper_bound": date_upper_bound,
-                "date_lower_bound": date_lower_bound,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "metadata": metadata,
-                "counterparty_id": counterparty_id,
-                "remittance_information": remittance_information,
-            },
+            body=maybe_transform(
+                {
+                    "amount_upper_bound": amount_upper_bound,
+                    "amount_lower_bound": amount_lower_bound,
+                    "direction": direction,
+                    "internal_account_id": internal_account_id,
+                    "type": type,
+                    "currency": currency,
+                    "date_upper_bound": date_upper_bound,
+                    "date_lower_bound": date_lower_bound,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "metadata": metadata,
+                    "counterparty_id": counterparty_id,
+                    "remittance_information": remittance_information,
+                },
+                expected_payment_update_params.ExpectedPaymentUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExpectedPayment,
         )
 
     def list(
         self,
         *,
@@ -244,16 +254,16 @@
             "sepa",
             "signet",
             "wire",
         ]
         | NotGiven = NOT_GIVEN,
         counterparty_id: str | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        created_at_lower_bound: str | NotGiven = NOT_GIVEN,
-        created_at_upper_bound: str | NotGiven = NOT_GIVEN,
+        created_at_lower_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
+        created_at_upper_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[ExpectedPayment]:
         """
@@ -288,26 +298,29 @@
         return self._get_api_list(
             "/api/expected_payments",
             page=SyncPage[ExpectedPayment],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "status": status,
-                    "internal_account_id": internal_account_id,
-                    "direction": direction,
-                    "type": type,
-                    "counterparty_id": counterparty_id,
-                    "metadata": metadata,
-                    "created_at_lower_bound": created_at_lower_bound,
-                    "created_at_upper_bound": created_at_upper_bound,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "status": status,
+                        "internal_account_id": internal_account_id,
+                        "direction": direction,
+                        "type": type,
+                        "counterparty_id": counterparty_id,
+                        "metadata": metadata,
+                        "created_at_lower_bound": created_at_lower_bound,
+                        "created_at_upper_bound": created_at_upper_bound,
+                    },
+                    expected_payment_list_params.ExpectedPaymentListParams,
+                ),
             ),
             model=ExpectedPayment,
         )
 
     def delete(
         self,
         id: str,
@@ -332,16 +345,16 @@
         *,
         amount_upper_bound: int,
         amount_lower_bound: int,
         direction: Literal["credit", "debit"],
         internal_account_id: str,
         type: ExpectedPaymentType | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        date_upper_bound: Optional[str] | NotGiven = NOT_GIVEN,
-        date_lower_bound: Optional[str] | NotGiven = NOT_GIVEN,
+        date_upper_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
+        date_lower_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         counterparty_id: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         line_items: List[expected_payment_create_params.LineItem] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -394,30 +407,33 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/expected_payments",
-            body={
-                "amount_upper_bound": amount_upper_bound,
-                "amount_lower_bound": amount_lower_bound,
-                "direction": direction,
-                "internal_account_id": internal_account_id,
-                "type": type,
-                "currency": currency,
-                "date_upper_bound": date_upper_bound,
-                "date_lower_bound": date_lower_bound,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "metadata": metadata,
-                "counterparty_id": counterparty_id,
-                "remittance_information": remittance_information,
-                "line_items": line_items,
-            },
+            body=maybe_transform(
+                {
+                    "amount_upper_bound": amount_upper_bound,
+                    "amount_lower_bound": amount_lower_bound,
+                    "direction": direction,
+                    "internal_account_id": internal_account_id,
+                    "type": type,
+                    "currency": currency,
+                    "date_upper_bound": date_upper_bound,
+                    "date_lower_bound": date_lower_bound,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "metadata": metadata,
+                    "counterparty_id": counterparty_id,
+                    "remittance_information": remittance_information,
+                    "line_items": line_items,
+                },
+                expected_payment_create_params.ExpectedPaymentCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExpectedPayment,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -441,16 +457,16 @@
         *,
         amount_upper_bound: int | NotGiven = NOT_GIVEN,
         amount_lower_bound: int | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         internal_account_id: str | NotGiven = NOT_GIVEN,
         type: ExpectedPaymentType | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        date_upper_bound: Optional[str] | NotGiven = NOT_GIVEN,
-        date_lower_bound: Optional[str] | NotGiven = NOT_GIVEN,
+        date_upper_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
+        date_lower_bound: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         counterparty_id: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -502,29 +518,32 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/expected_payments/{id}",
-            body={
-                "amount_upper_bound": amount_upper_bound,
-                "amount_lower_bound": amount_lower_bound,
-                "direction": direction,
-                "internal_account_id": internal_account_id,
-                "type": type,
-                "currency": currency,
-                "date_upper_bound": date_upper_bound,
-                "date_lower_bound": date_lower_bound,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "metadata": metadata,
-                "counterparty_id": counterparty_id,
-                "remittance_information": remittance_information,
-            },
+            body=maybe_transform(
+                {
+                    "amount_upper_bound": amount_upper_bound,
+                    "amount_lower_bound": amount_lower_bound,
+                    "direction": direction,
+                    "internal_account_id": internal_account_id,
+                    "type": type,
+                    "currency": currency,
+                    "date_upper_bound": date_upper_bound,
+                    "date_lower_bound": date_lower_bound,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "metadata": metadata,
+                    "counterparty_id": counterparty_id,
+                    "remittance_information": remittance_information,
+                },
+                expected_payment_update_params.ExpectedPaymentUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExpectedPayment,
         )
 
     def list(
         self,
         *,
@@ -551,16 +570,16 @@
             "sepa",
             "signet",
             "wire",
         ]
         | NotGiven = NOT_GIVEN,
         counterparty_id: str | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        created_at_lower_bound: str | NotGiven = NOT_GIVEN,
-        created_at_upper_bound: str | NotGiven = NOT_GIVEN,
+        created_at_lower_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
+        created_at_upper_bound: Union[str, datetime] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[ExpectedPayment, AsyncPage[ExpectedPayment]]:
         """
@@ -595,26 +614,29 @@
         return self._get_api_list(
             "/api/expected_payments",
             page=AsyncPage[ExpectedPayment],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "status": status,
-                    "internal_account_id": internal_account_id,
-                    "direction": direction,
-                    "type": type,
-                    "counterparty_id": counterparty_id,
-                    "metadata": metadata,
-                    "created_at_lower_bound": created_at_lower_bound,
-                    "created_at_upper_bound": created_at_upper_bound,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "status": status,
+                        "internal_account_id": internal_account_id,
+                        "direction": direction,
+                        "type": type,
+                        "counterparty_id": counterparty_id,
+                        "metadata": metadata,
+                        "created_at_lower_bound": created_at_lower_bound,
+                        "created_at_upper_bound": created_at_upper_bound,
+                    },
+                    expected_payment_list_params.ExpectedPaymentListParams,
+                ),
             ),
             model=ExpectedPayment,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/external_accounts.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/external_accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 from typing import Dict, List, Optional
 from typing_extensions import Literal
 
 from ..types import (
     ExternalAccount,
     ExternalAccountType,
     shared_params,
+    external_account_list_params,
     external_account_create_params,
     external_account_update_params,
+    external_account_verify_params,
+    external_account_complete_verification_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["ExternalAccounts", "AsyncExternalAccounts"]
 
 
@@ -67,28 +71,31 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/external_accounts",
-            body={
-                "account_type": account_type,
-                "party_type": party_type,
-                "party_address": party_address,
-                "name": name,
-                "counterparty_id": counterparty_id,
-                "account_details": account_details,
-                "routing_details": routing_details,
-                "metadata": metadata,
-                "party_name": party_name,
-                "party_identifier": party_identifier,
-                "plaid_processor_token": plaid_processor_token,
-                "contact_details": contact_details,
-            },
+            body=maybe_transform(
+                {
+                    "account_type": account_type,
+                    "party_type": party_type,
+                    "party_address": party_address,
+                    "name": name,
+                    "counterparty_id": counterparty_id,
+                    "account_details": account_details,
+                    "routing_details": routing_details,
+                    "metadata": metadata,
+                    "party_name": party_name,
+                    "party_identifier": party_identifier,
+                    "plaid_processor_token": plaid_processor_token,
+                    "contact_details": contact_details,
+                },
+                external_account_create_params.ExternalAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
     def retrieve(
         self,
         id: str,
@@ -143,23 +150,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/external_accounts/{id}",
-            body={
-                "party_type": party_type,
-                "account_type": account_type,
-                "counterparty_id": counterparty_id,
-                "name": name,
-                "party_name": party_name,
-                "party_address": party_address,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "party_type": party_type,
+                    "account_type": account_type,
+                    "counterparty_id": counterparty_id,
+                    "name": name,
+                    "party_name": party_name,
+                    "party_address": party_address,
+                    "metadata": metadata,
+                },
+                external_account_update_params.ExternalAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
     def list(
         self,
         *,
@@ -193,21 +203,24 @@
         return self._get_api_list(
             "/api/external_accounts",
             page=SyncPage[ExternalAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "party_name": party_name,
-                    "counterparty_id": counterparty_id,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "party_name": party_name,
+                        "counterparty_id": counterparty_id,
+                        "metadata": metadata,
+                    },
+                    external_account_list_params.ExternalAccountListParams,
+                ),
             ),
             model=ExternalAccount,
         )
 
     def delete(
         self,
         id: str,
@@ -245,15 +258,18 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             f"/api/external_accounts/{id}/complete_verification",
-            body={"amounts": amounts},
+            body=maybe_transform(
+                {"amounts": amounts},
+                external_account_complete_verification_params.ExternalAccountCompleteVerificationParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
     def verify(
         self,
         id: str,
@@ -300,19 +316,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             f"/api/external_accounts/{id}/verify",
-            body={
-                "originating_account_id": originating_account_id,
-                "payment_type": payment_type,
-                "currency": currency,
-            },
+            body=maybe_transform(
+                {
+                    "originating_account_id": originating_account_id,
+                    "payment_type": payment_type,
+                    "currency": currency,
+                },
+                external_account_verify_params.ExternalAccountVerifyParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
 
 class AsyncExternalAccounts(AsyncAPIResource):
     async def create(
@@ -361,28 +380,31 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/external_accounts",
-            body={
-                "account_type": account_type,
-                "party_type": party_type,
-                "party_address": party_address,
-                "name": name,
-                "counterparty_id": counterparty_id,
-                "account_details": account_details,
-                "routing_details": routing_details,
-                "metadata": metadata,
-                "party_name": party_name,
-                "party_identifier": party_identifier,
-                "plaid_processor_token": plaid_processor_token,
-                "contact_details": contact_details,
-            },
+            body=maybe_transform(
+                {
+                    "account_type": account_type,
+                    "party_type": party_type,
+                    "party_address": party_address,
+                    "name": name,
+                    "counterparty_id": counterparty_id,
+                    "account_details": account_details,
+                    "routing_details": routing_details,
+                    "metadata": metadata,
+                    "party_name": party_name,
+                    "party_identifier": party_identifier,
+                    "plaid_processor_token": plaid_processor_token,
+                    "contact_details": contact_details,
+                },
+                external_account_create_params.ExternalAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -437,23 +459,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/external_accounts/{id}",
-            body={
-                "party_type": party_type,
-                "account_type": account_type,
-                "counterparty_id": counterparty_id,
-                "name": name,
-                "party_name": party_name,
-                "party_address": party_address,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "party_type": party_type,
+                    "account_type": account_type,
+                    "counterparty_id": counterparty_id,
+                    "name": name,
+                    "party_name": party_name,
+                    "party_address": party_address,
+                    "metadata": metadata,
+                },
+                external_account_update_params.ExternalAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
     def list(
         self,
         *,
@@ -487,21 +512,24 @@
         return self._get_api_list(
             "/api/external_accounts",
             page=AsyncPage[ExternalAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "party_name": party_name,
-                    "counterparty_id": counterparty_id,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "party_name": party_name,
+                        "counterparty_id": counterparty_id,
+                        "metadata": metadata,
+                    },
+                    external_account_list_params.ExternalAccountListParams,
+                ),
             ),
             model=ExternalAccount,
         )
 
     async def delete(
         self,
         id: str,
@@ -539,15 +567,18 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             f"/api/external_accounts/{id}/complete_verification",
-            body={"amounts": amounts},
+            body=maybe_transform(
+                {"amounts": amounts},
+                external_account_complete_verification_params.ExternalAccountCompleteVerificationParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
 
     async def verify(
         self,
         id: str,
@@ -594,15 +625,18 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             f"/api/external_accounts/{id}/verify",
-            body={
-                "originating_account_id": originating_account_id,
-                "payment_type": payment_type,
-                "currency": currency,
-            },
+            body=maybe_transform(
+                {
+                    "originating_account_id": originating_account_id,
+                    "payment_type": payment_type,
+                    "currency": currency,
+                },
+                external_account_verify_params.ExternalAccountVerifyParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ExternalAccount,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/incoming_payment_details.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/incoming_payment_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import date
 from typing_extensions import Literal
 
-from ..types import IncomingPaymentDetail, shared, shared_params
+from ..types import (
+    IncomingPaymentDetail,
+    shared,
+    shared_params,
+    incoming_payment_detail_list_params,
+    incoming_payment_detail_update_params,
+    incoming_payment_detail_create_async_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["IncomingPaymentDetails", "AsyncIncomingPaymentDetails"]
 
 
@@ -54,29 +63,31 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/incoming_payment_details/{id}",
-            body={"metadata": metadata},
+            body=maybe_transform(
+                {"metadata": metadata}, incoming_payment_detail_update_params.IncomingPaymentDetailUpdateParams
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=IncomingPaymentDetail,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         status: Literal["completed", "pending", "returned"] | NotGiven = NOT_GIVEN,
         type: Literal["ach", "book", "check", "eft", "interac", "rtp", "sepa", "signet", "wire"] | NotGiven = NOT_GIVEN,
-        as_of_date_start: str | NotGiven = NOT_GIVEN,
-        as_of_date_end: str | NotGiven = NOT_GIVEN,
+        as_of_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        as_of_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         virtual_account_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -115,39 +126,42 @@
         return self._get_api_list(
             "/api/incoming_payment_details",
             page=SyncPage[IncomingPaymentDetail],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "direction": direction,
-                    "status": status,
-                    "type": type,
-                    "as_of_date_start": as_of_date_start,
-                    "as_of_date_end": as_of_date_end,
-                    "metadata": metadata,
-                    "virtual_account_id": virtual_account_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "direction": direction,
+                        "status": status,
+                        "type": type,
+                        "as_of_date_start": as_of_date_start,
+                        "as_of_date_end": as_of_date_end,
+                        "metadata": metadata,
+                        "virtual_account_id": virtual_account_id,
+                    },
+                    incoming_payment_detail_list_params.IncomingPaymentDetailListParams,
+                ),
             ),
             model=IncomingPaymentDetail,
         )
 
     def create_async(
         self,
         *,
         type: Literal["ach", "book", "check", "eft", "interac", "rtp", "sepa", "signet", "wire"] | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         amount: int | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
         internal_account_id: str | NotGiven = NOT_GIVEN,
         virtual_account_id: Optional[str] | NotGiven = NOT_GIVEN,
-        as_of_date: Optional[str] | NotGiven = NOT_GIVEN,
+        as_of_date: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> shared.AsyncResponse:
         """
@@ -174,23 +188,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/simulations/incoming_payment_details/create_async",
-            body={
-                "type": type,
-                "direction": direction,
-                "amount": amount,
-                "currency": currency,
-                "internal_account_id": internal_account_id,
-                "virtual_account_id": virtual_account_id,
-                "as_of_date": as_of_date,
-            },
+            body=maybe_transform(
+                {
+                    "type": type,
+                    "direction": direction,
+                    "amount": amount,
+                    "currency": currency,
+                    "internal_account_id": internal_account_id,
+                    "virtual_account_id": virtual_account_id,
+                    "as_of_date": as_of_date,
+                },
+                incoming_payment_detail_create_async_params.IncomingPaymentDetailCreateAsyncParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=shared.AsyncResponse,
         )
 
 
 class AsyncIncomingPaymentDetails(AsyncAPIResource):
     async def retrieve(
@@ -232,29 +249,31 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/incoming_payment_details/{id}",
-            body={"metadata": metadata},
+            body=maybe_transform(
+                {"metadata": metadata}, incoming_payment_detail_update_params.IncomingPaymentDetailUpdateParams
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=IncomingPaymentDetail,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         status: Literal["completed", "pending", "returned"] | NotGiven = NOT_GIVEN,
         type: Literal["ach", "book", "check", "eft", "interac", "rtp", "sepa", "signet", "wire"] | NotGiven = NOT_GIVEN,
-        as_of_date_start: str | NotGiven = NOT_GIVEN,
-        as_of_date_end: str | NotGiven = NOT_GIVEN,
+        as_of_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        as_of_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         virtual_account_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -293,39 +312,42 @@
         return self._get_api_list(
             "/api/incoming_payment_details",
             page=AsyncPage[IncomingPaymentDetail],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "direction": direction,
-                    "status": status,
-                    "type": type,
-                    "as_of_date_start": as_of_date_start,
-                    "as_of_date_end": as_of_date_end,
-                    "metadata": metadata,
-                    "virtual_account_id": virtual_account_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "direction": direction,
+                        "status": status,
+                        "type": type,
+                        "as_of_date_start": as_of_date_start,
+                        "as_of_date_end": as_of_date_end,
+                        "metadata": metadata,
+                        "virtual_account_id": virtual_account_id,
+                    },
+                    incoming_payment_detail_list_params.IncomingPaymentDetailListParams,
+                ),
             ),
             model=IncomingPaymentDetail,
         )
 
     async def create_async(
         self,
         *,
         type: Literal["ach", "book", "check", "eft", "interac", "rtp", "sepa", "signet", "wire"] | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         amount: int | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
         internal_account_id: str | NotGiven = NOT_GIVEN,
         virtual_account_id: Optional[str] | NotGiven = NOT_GIVEN,
-        as_of_date: Optional[str] | NotGiven = NOT_GIVEN,
+        as_of_date: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> shared.AsyncResponse:
         """
@@ -352,19 +374,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/simulations/incoming_payment_details/create_async",
-            body={
-                "type": type,
-                "direction": direction,
-                "amount": amount,
-                "currency": currency,
-                "internal_account_id": internal_account_id,
-                "virtual_account_id": virtual_account_id,
-                "as_of_date": as_of_date,
-            },
+            body=maybe_transform(
+                {
+                    "type": type,
+                    "direction": direction,
+                    "amount": amount,
+                    "currency": currency,
+                    "internal_account_id": internal_account_id,
+                    "virtual_account_id": virtual_account_id,
+                    "as_of_date": as_of_date,
+                },
+                incoming_payment_detail_create_async_params.IncomingPaymentDetailCreateAsyncParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=shared.AsyncResponse,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/internal_accounts/balance_reports.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/internal_accounts/balance_reports.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Union, Optional
+from datetime import date
 from typing_extensions import Literal
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import AsyncPaginator, make_request_options
-from ...types.internal_accounts import BalanceReport
+from ...types.internal_accounts import BalanceReport, balance_report_list_params
 
 __all__ = ["BalanceReports", "AsyncBalanceReports"]
 
 
 class BalanceReports(SyncAPIResource):
     def retrieve(
         self,
@@ -33,15 +35,15 @@
             cast_to=BalanceReport,
         )
 
     def list(
         self,
         internal_account_id: str,
         *,
-        as_of_date: str | NotGiven = NOT_GIVEN,
+        as_of_date: Union[str, date] | NotGiven = NOT_GIVEN,
         balance_report_type: Literal["intraday", "other", "previous_day", "real_time"] | NotGiven = NOT_GIVEN,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -65,20 +67,23 @@
         return self._get_api_list(
             f"/api/internal_accounts/{internal_account_id}/balance_reports",
             page=SyncPage[BalanceReport],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "as_of_date": as_of_date,
-                    "balance_report_type": balance_report_type,
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "as_of_date": as_of_date,
+                        "balance_report_type": balance_report_type,
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    balance_report_list_params.BalanceReportListParams,
+                ),
             ),
             model=BalanceReport,
         )
 
 
 class AsyncBalanceReports(AsyncAPIResource):
     async def retrieve(
@@ -99,15 +104,15 @@
             cast_to=BalanceReport,
         )
 
     def list(
         self,
         internal_account_id: str,
         *,
-        as_of_date: str | NotGiven = NOT_GIVEN,
+        as_of_date: Union[str, date] | NotGiven = NOT_GIVEN,
         balance_report_type: Literal["intraday", "other", "previous_day", "real_time"] | NotGiven = NOT_GIVEN,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -131,16 +136,19 @@
         return self._get_api_list(
             f"/api/internal_accounts/{internal_account_id}/balance_reports",
             page=AsyncPage[BalanceReport],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "as_of_date": as_of_date,
-                    "balance_report_type": balance_report_type,
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "as_of_date": as_of_date,
+                        "balance_report_type": balance_report_type,
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    balance_report_list_params.BalanceReportListParams,
+                ),
             ),
             model=BalanceReport,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/internal_accounts/internal_accounts.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/internal_accounts/internal_accounts.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict, Optional
 from typing_extensions import Literal
 
-from ...types import InternalAccount, shared_params, internal_account_create_params
+from ...types import (
+    InternalAccount,
+    shared_params,
+    internal_account_list_params,
+    internal_account_create_params,
+    internal_account_update_params,
+)
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import AsyncPaginator, make_request_options
 from .balance_reports import BalanceReports, AsyncBalanceReports
 
 if TYPE_CHECKING:
     from ..._client import ModernTreasury, AsyncModernTreasury
@@ -67,24 +74,27 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/internal_accounts",
-            body={
-                "connection_id": connection_id,
-                "name": name,
-                "party_name": party_name,
-                "party_address": party_address,
-                "currency": currency,
-                "entity_id": entity_id,
-                "parent_account_id": parent_account_id,
-                "counterparty_id": counterparty_id,
-            },
+            body=maybe_transform(
+                {
+                    "connection_id": connection_id,
+                    "name": name,
+                    "party_name": party_name,
+                    "party_address": party_address,
+                    "currency": currency,
+                    "entity_id": entity_id,
+                    "parent_account_id": parent_account_id,
+                    "counterparty_id": counterparty_id,
+                },
+                internal_account_create_params.InternalAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=InternalAccount,
         )
 
     def retrieve(
         self,
         id: str,
@@ -133,20 +143,23 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/internal_accounts/{id}",
-            body={
-                "name": name,
-                "metadata": metadata,
-                "parent_account_id": parent_account_id,
-                "counterparty_id": counterparty_id,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "metadata": metadata,
+                    "parent_account_id": parent_account_id,
+                    "counterparty_id": counterparty_id,
+                },
+                internal_account_update_params.InternalAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=InternalAccount,
         )
 
     def list(
         self,
         *,
@@ -204,22 +217,25 @@
         return self._get_api_list(
             "/api/internal_accounts",
             page=SyncPage[InternalAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "currency": currency,
-                    "payment_type": payment_type,
-                    "payment_direction": payment_direction,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "currency": currency,
+                        "payment_type": payment_type,
+                        "payment_direction": payment_direction,
+                        "metadata": metadata,
+                    },
+                    internal_account_list_params.InternalAccountListParams,
+                ),
             ),
             model=InternalAccount,
         )
 
 
 class AsyncInternalAccounts(AsyncAPIResource):
     balance_reports: AsyncBalanceReports
@@ -270,24 +286,27 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/internal_accounts",
-            body={
-                "connection_id": connection_id,
-                "name": name,
-                "party_name": party_name,
-                "party_address": party_address,
-                "currency": currency,
-                "entity_id": entity_id,
-                "parent_account_id": parent_account_id,
-                "counterparty_id": counterparty_id,
-            },
+            body=maybe_transform(
+                {
+                    "connection_id": connection_id,
+                    "name": name,
+                    "party_name": party_name,
+                    "party_address": party_address,
+                    "currency": currency,
+                    "entity_id": entity_id,
+                    "parent_account_id": parent_account_id,
+                    "counterparty_id": counterparty_id,
+                },
+                internal_account_create_params.InternalAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=InternalAccount,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -336,20 +355,23 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/internal_accounts/{id}",
-            body={
-                "name": name,
-                "metadata": metadata,
-                "parent_account_id": parent_account_id,
-                "counterparty_id": counterparty_id,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "metadata": metadata,
+                    "parent_account_id": parent_account_id,
+                    "counterparty_id": counterparty_id,
+                },
+                internal_account_update_params.InternalAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=InternalAccount,
         )
 
     def list(
         self,
         *,
@@ -407,18 +429,21 @@
         return self._get_api_list(
             "/api/internal_accounts",
             page=AsyncPage[InternalAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "currency": currency,
-                    "payment_type": payment_type,
-                    "payment_direction": payment_direction,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "currency": currency,
+                        "payment_type": payment_type,
+                        "payment_direction": payment_direction,
+                        "metadata": metadata,
+                    },
+                    internal_account_list_params.InternalAccountListParams,
+                ),
             ),
             model=InternalAccount,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledger_account_categories.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledger_account_categories.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Dict, Optional
 from typing_extensions import Literal
 
-from ..types import LedgerAccountCategory, ledger_account_category_retrieve_params
+from ..types import (
+    LedgerAccountCategory,
+    ledger_account_category_list_params,
+    ledger_account_category_create_params,
+    ledger_account_category_update_params,
+    ledger_account_category_retrieve_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["LedgerAccountCategories", "AsyncLedgerAccountCategories"]
 
 
@@ -54,23 +61,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/ledger_account_categories",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-                "currency": currency,
-                "currency_exponent": currency_exponent,
-                "ledger_id": ledger_id,
-                "normal_balance": normal_balance,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                    "currency": currency,
+                    "currency_exponent": currency_exponent,
+                    "ledger_id": ledger_id,
+                    "normal_balance": normal_balance,
+                },
+                ledger_account_category_create_params.LedgerAccountCategoryCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountCategory,
         )
 
     def retrieve(
         self,
         id: str,
@@ -99,15 +109,17 @@
         """
         return self._get(
             f"/api/ledger_account_categories/{id}",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={"balances": balances},
+                query=maybe_transform(
+                    {"balances": balances}, ledger_account_category_retrieve_params.LedgerAccountCategoryRetrieveParams
+                ),
             ),
             cast_to=LedgerAccountCategory,
         )
 
     def update(
         self,
         id: str,
@@ -136,19 +148,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/ledger_account_categories/{id}",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                },
+                ledger_account_category_update_params.LedgerAccountCategoryUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountCategory,
         )
 
     def list(
         self,
         *,
@@ -183,22 +198,25 @@
         return self._get_api_list(
             "/api/ledger_account_categories",
             page=SyncPage[LedgerAccountCategory],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "name": name,
-                    "ledger_id": ledger_id,
-                    "parent_ledger_account_category_id": parent_ledger_account_category_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "name": name,
+                        "ledger_id": ledger_id,
+                        "parent_ledger_account_category_id": parent_ledger_account_category_id,
+                    },
+                    ledger_account_category_list_params.LedgerAccountCategoryListParams,
+                ),
             ),
             model=LedgerAccountCategory,
         )
 
     def delete(
         self,
         id: str,
@@ -333,23 +351,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/ledger_account_categories",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-                "currency": currency,
-                "currency_exponent": currency_exponent,
-                "ledger_id": ledger_id,
-                "normal_balance": normal_balance,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                    "currency": currency,
+                    "currency_exponent": currency_exponent,
+                    "ledger_id": ledger_id,
+                    "normal_balance": normal_balance,
+                },
+                ledger_account_category_create_params.LedgerAccountCategoryCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountCategory,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -378,15 +399,17 @@
         """
         return await self._get(
             f"/api/ledger_account_categories/{id}",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={"balances": balances},
+                query=maybe_transform(
+                    {"balances": balances}, ledger_account_category_retrieve_params.LedgerAccountCategoryRetrieveParams
+                ),
             ),
             cast_to=LedgerAccountCategory,
         )
 
     async def update(
         self,
         id: str,
@@ -415,19 +438,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/ledger_account_categories/{id}",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                },
+                ledger_account_category_update_params.LedgerAccountCategoryUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountCategory,
         )
 
     def list(
         self,
         *,
@@ -462,22 +488,25 @@
         return self._get_api_list(
             "/api/ledger_account_categories",
             page=AsyncPage[LedgerAccountCategory],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "name": name,
-                    "ledger_id": ledger_id,
-                    "parent_ledger_account_category_id": parent_ledger_account_category_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "name": name,
+                        "ledger_id": ledger_id,
+                        "parent_ledger_account_category_id": parent_ledger_account_category_id,
+                    },
+                    ledger_account_category_list_params.LedgerAccountCategoryListParams,
+                ),
             ),
             model=LedgerAccountCategory,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledger_account_payouts.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledger_account_payouts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Dict, Optional
 from typing_extensions import Literal
 
-from ..types import LedgerAccountPayout
+from ..types import (
+    LedgerAccountPayout,
+    ledger_account_payout_list_params,
+    ledger_account_payout_create_params,
+    ledger_account_payout_update_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["LedgerAccountPayouts", "AsyncLedgerAccountPayouts"]
 
 
@@ -56,22 +62,25 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/ledger_account_payouts",
-            body={
-                "description": description,
-                "status": status,
-                "payout_ledger_account_id": payout_ledger_account_id,
-                "funding_ledger_account_id": funding_ledger_account_id,
-                "effective_at_upper_bound": effective_at_upper_bound,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "payout_ledger_account_id": payout_ledger_account_id,
+                    "funding_ledger_account_id": funding_ledger_account_id,
+                    "effective_at_upper_bound": effective_at_upper_bound,
+                    "metadata": metadata,
+                },
+                ledger_account_payout_create_params.LedgerAccountPayoutCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountPayout,
         )
 
     def update(
         self,
         id: str,
@@ -101,19 +110,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/ledger_account_payouts/{id}",
-            body={
-                "description": description,
-                "status": status,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "metadata": metadata,
+                },
+                ledger_account_payout_update_params.LedgerAccountPayoutUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountPayout,
         )
 
     def list(
         self,
         *,
@@ -139,19 +151,22 @@
         return self._get_api_list(
             "/api/ledger_account_payouts",
             page=SyncPage[LedgerAccountPayout],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "payout_ledger_account_id": payout_ledger_account_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "payout_ledger_account_id": payout_ledger_account_id,
+                    },
+                    ledger_account_payout_list_params.LedgerAccountPayoutListParams,
+                ),
             ),
             model=LedgerAccountPayout,
         )
 
     def retireve(
         self,
         id: str,
@@ -212,22 +227,25 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/ledger_account_payouts",
-            body={
-                "description": description,
-                "status": status,
-                "payout_ledger_account_id": payout_ledger_account_id,
-                "funding_ledger_account_id": funding_ledger_account_id,
-                "effective_at_upper_bound": effective_at_upper_bound,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "payout_ledger_account_id": payout_ledger_account_id,
+                    "funding_ledger_account_id": funding_ledger_account_id,
+                    "effective_at_upper_bound": effective_at_upper_bound,
+                    "metadata": metadata,
+                },
+                ledger_account_payout_create_params.LedgerAccountPayoutCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountPayout,
         )
 
     async def update(
         self,
         id: str,
@@ -257,19 +275,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/ledger_account_payouts/{id}",
-            body={
-                "description": description,
-                "status": status,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "metadata": metadata,
+                },
+                ledger_account_payout_update_params.LedgerAccountPayoutUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccountPayout,
         )
 
     def list(
         self,
         *,
@@ -295,19 +316,22 @@
         return self._get_api_list(
             "/api/ledger_account_payouts",
             page=AsyncPage[LedgerAccountPayout],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "payout_ledger_account_id": payout_ledger_account_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "payout_ledger_account_id": payout_ledger_account_id,
+                    },
+                    ledger_account_payout_list_params.LedgerAccountPayoutListParams,
+                ),
             ),
             model=LedgerAccountPayout,
         )
 
     async def retireve(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledger_accounts.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledger_accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from ..types import (
     LedgerAccount,
     ledger_account_list_params,
+    ledger_account_create_params,
+    ledger_account_update_params,
     ledger_account_retrieve_params,
 )
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["LedgerAccounts", "AsyncLedgerAccounts"]
 
 
@@ -58,23 +62,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/ledger_accounts",
-            body={
-                "name": name,
-                "description": description,
-                "normal_balance": normal_balance,
-                "ledger_id": ledger_id,
-                "currency": currency,
-                "currency_exponent": currency_exponent,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "normal_balance": normal_balance,
+                    "ledger_id": ledger_id,
+                    "currency": currency,
+                    "currency_exponent": currency_exponent,
+                    "metadata": metadata,
+                },
+                ledger_account_create_params.LedgerAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccount,
         )
 
     def retrieve(
         self,
         id: str,
@@ -103,15 +110,17 @@
         """
         return self._get(
             f"/api/ledger_accounts/{id}",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={"balances": balances},
+                query=maybe_transform(
+                    {"balances": balances}, ledger_account_retrieve_params.LedgerAccountRetrieveParams
+                ),
             ),
             cast_to=LedgerAccount,
         )
 
     def update(
         self,
         id: str,
@@ -143,35 +152,38 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/ledger_accounts/{id}",
-            body={
-                "name": name,
-                "description": description,
-                "normal_balance": normal_balance,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "normal_balance": normal_balance,
+                    "metadata": metadata,
+                },
+                ledger_account_update_params.LedgerAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccount,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         id: str | NotGiven = NOT_GIVEN,
         name: str | NotGiven = NOT_GIVEN,
         ledger_id: str | NotGiven = NOT_GIVEN,
         balances: ledger_account_list_params.Balances | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         ledger_account_category_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[LedgerAccount]:
@@ -201,25 +213,28 @@
         return self._get_api_list(
             "/api/ledger_accounts",
             page=SyncPage[LedgerAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "id": id,
-                    "name": name,
-                    "ledger_id": ledger_id,
-                    "balances": balances,
-                    "updated_at": updated_at,
-                    "ledger_account_category_id": ledger_account_category_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "id": id,
+                        "name": name,
+                        "ledger_id": ledger_id,
+                        "balances": balances,
+                        "updated_at": updated_at,
+                        "ledger_account_category_id": ledger_account_category_id,
+                    },
+                    ledger_account_list_params.LedgerAccountListParams,
+                ),
             ),
             model=LedgerAccount,
         )
 
     def delete(
         self,
         id: str,
@@ -278,23 +293,26 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/ledger_accounts",
-            body={
-                "name": name,
-                "description": description,
-                "normal_balance": normal_balance,
-                "ledger_id": ledger_id,
-                "currency": currency,
-                "currency_exponent": currency_exponent,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "normal_balance": normal_balance,
+                    "ledger_id": ledger_id,
+                    "currency": currency,
+                    "currency_exponent": currency_exponent,
+                    "metadata": metadata,
+                },
+                ledger_account_create_params.LedgerAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccount,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -323,15 +341,17 @@
         """
         return await self._get(
             f"/api/ledger_accounts/{id}",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={"balances": balances},
+                query=maybe_transform(
+                    {"balances": balances}, ledger_account_retrieve_params.LedgerAccountRetrieveParams
+                ),
             ),
             cast_to=LedgerAccount,
         )
 
     async def update(
         self,
         id: str,
@@ -363,35 +383,38 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/ledger_accounts/{id}",
-            body={
-                "name": name,
-                "description": description,
-                "normal_balance": normal_balance,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "normal_balance": normal_balance,
+                    "metadata": metadata,
+                },
+                ledger_account_update_params.LedgerAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerAccount,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         id: str | NotGiven = NOT_GIVEN,
         name: str | NotGiven = NOT_GIVEN,
         ledger_id: str | NotGiven = NOT_GIVEN,
         balances: ledger_account_list_params.Balances | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         ledger_account_category_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[LedgerAccount, AsyncPage[LedgerAccount]]:
@@ -421,25 +444,28 @@
         return self._get_api_list(
             "/api/ledger_accounts",
             page=AsyncPage[LedgerAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "id": id,
-                    "name": name,
-                    "ledger_id": ledger_id,
-                    "balances": balances,
-                    "updated_at": updated_at,
-                    "ledger_account_category_id": ledger_account_category_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "id": id,
+                        "name": name,
+                        "ledger_id": ledger_id,
+                        "balances": balances,
+                        "updated_at": updated_at,
+                        "ledger_account_category_id": ledger_account_category_id,
+                    },
+                    ledger_account_list_params.LedgerAccountListParams,
+                ),
             ),
             model=LedgerAccount,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledger_entries.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledger_entries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
-from ..types import LedgerEntry
+from ..types import LedgerEntry, ledger_entry_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["LedgerEntries", "AsyncLedgerEntries"]
 
 
@@ -35,17 +37,17 @@
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         ledger_account_id: str | NotGiven = NOT_GIVEN,
         ledger_transaction_id: str | NotGiven = NOT_GIVEN,
-        effective_date: Dict[str, str] | NotGiven = NOT_GIVEN,
+        effective_date: Dict[str, Union[str, date]] | NotGiven = NOT_GIVEN,
         effective_at: Dict[str, str] | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         ledger_account_lock_version: Dict[str, int] | NotGiven = NOT_GIVEN,
         ledger_account_category_id: str | NotGiven = NOT_GIVEN,
         show_deleted: bool | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         status: Literal["pending", "posted", "archived"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -95,28 +97,31 @@
         return self._get_api_list(
             "/api/ledger_entries",
             page=SyncPage[LedgerEntry],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "ledger_account_id": ledger_account_id,
-                    "ledger_transaction_id": ledger_transaction_id,
-                    "effective_date": effective_date,
-                    "effective_at": effective_at,
-                    "updated_at": updated_at,
-                    "ledger_account_lock_version": ledger_account_lock_version,
-                    "ledger_account_category_id": ledger_account_category_id,
-                    "show_deleted": show_deleted,
-                    "direction": direction,
-                    "status": status,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "ledger_account_id": ledger_account_id,
+                        "ledger_transaction_id": ledger_transaction_id,
+                        "effective_date": effective_date,
+                        "effective_at": effective_at,
+                        "updated_at": updated_at,
+                        "ledger_account_lock_version": ledger_account_lock_version,
+                        "ledger_account_category_id": ledger_account_category_id,
+                        "show_deleted": show_deleted,
+                        "direction": direction,
+                        "status": status,
+                    },
+                    ledger_entry_list_params.LedgerEntryListParams,
+                ),
             ),
             model=LedgerEntry,
         )
 
 
 class AsyncLedgerEntries(AsyncAPIResource):
     async def retrieve(
@@ -139,17 +144,17 @@
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         ledger_account_id: str | NotGiven = NOT_GIVEN,
         ledger_transaction_id: str | NotGiven = NOT_GIVEN,
-        effective_date: Dict[str, str] | NotGiven = NOT_GIVEN,
+        effective_date: Dict[str, Union[str, date]] | NotGiven = NOT_GIVEN,
         effective_at: Dict[str, str] | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         ledger_account_lock_version: Dict[str, int] | NotGiven = NOT_GIVEN,
         ledger_account_category_id: str | NotGiven = NOT_GIVEN,
         show_deleted: bool | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         status: Literal["pending", "posted", "archived"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -199,24 +204,27 @@
         return self._get_api_list(
             "/api/ledger_entries",
             page=AsyncPage[LedgerEntry],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "ledger_account_id": ledger_account_id,
-                    "ledger_transaction_id": ledger_transaction_id,
-                    "effective_date": effective_date,
-                    "effective_at": effective_at,
-                    "updated_at": updated_at,
-                    "ledger_account_lock_version": ledger_account_lock_version,
-                    "ledger_account_category_id": ledger_account_category_id,
-                    "show_deleted": show_deleted,
-                    "direction": direction,
-                    "status": status,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "ledger_account_id": ledger_account_id,
+                        "ledger_transaction_id": ledger_transaction_id,
+                        "effective_date": effective_date,
+                        "effective_at": effective_at,
+                        "updated_at": updated_at,
+                        "ledger_account_lock_version": ledger_account_lock_version,
+                        "ledger_account_category_id": ledger_account_category_id,
+                        "show_deleted": show_deleted,
+                        "direction": direction,
+                        "status": status,
+                    },
+                    ledger_entry_list_params.LedgerEntryListParams,
+                ),
             ),
             model=LedgerEntry,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledger_transactions/ledger_transactions.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledger_transactions/ledger_transactions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict, List, Optional
+from typing import TYPE_CHECKING, Dict, List, Union, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ...types import (
     LedgerTransaction,
+    ledger_transaction_list_params,
     ledger_transaction_create_params,
     ledger_transaction_update_params,
 )
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
 from .versions import Versions, AsyncVersions
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import AsyncPaginator, make_request_options
 
 if TYPE_CHECKING:
     from ..._client import ModernTreasury, AsyncModernTreasury
@@ -31,15 +34,15 @@
 
     def create(
         self,
         *,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         status: Literal["archived", "pending", "posted"] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        effective_date: str,
+        effective_date: Union[str, date],
         ledger_entries: List[ledger_transaction_create_params.LedgerEntry],
         external_id: str | NotGiven = NOT_GIVEN,
         ledgerable_type: Literal[
             "counterparty",
             "expected_payment",
             "incoming_payment_detail",
             "internal_account",
@@ -88,24 +91,27 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/ledger_transactions",
-            body={
-                "description": description,
-                "status": status,
-                "metadata": metadata,
-                "effective_date": effective_date,
-                "ledger_entries": ledger_entries,
-                "external_id": external_id,
-                "ledgerable_type": ledgerable_type,
-                "ledgerable_id": ledgerable_id,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "metadata": metadata,
+                    "effective_date": effective_date,
+                    "ledger_entries": ledger_entries,
+                    "external_id": external_id,
+                    "ledgerable_type": ledgerable_type,
+                    "ledgerable_id": ledgerable_id,
+                },
+                ledger_transaction_create_params.LedgerTransactionCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerTransaction,
         )
 
     def retrieve(
         self,
         id: str,
@@ -154,36 +160,39 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/ledger_transactions/{id}",
-            body={
-                "description": description,
-                "status": status,
-                "metadata": metadata,
-                "ledger_entries": ledger_entries,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "metadata": metadata,
+                    "ledger_entries": ledger_entries,
+                },
+                ledger_transaction_update_params.LedgerTransactionUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerTransaction,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         ledger_id: str | NotGiven = NOT_GIVEN,
         ledger_account_id: str | NotGiven = NOT_GIVEN,
         effective_at: Dict[str, str] | NotGiven = NOT_GIVEN,
-        effective_date: Dict[str, str] | NotGiven = NOT_GIVEN,
-        posted_at: Dict[str, str] | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        effective_date: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
+        posted_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         status: Literal["pending", "posted", "archived"] | NotGiven = NOT_GIVEN,
         external_id: str | NotGiven = NOT_GIVEN,
         ledger_account_category_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -222,28 +231,31 @@
         return self._get_api_list(
             "/api/ledger_transactions",
             page=SyncPage[LedgerTransaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "ledger_id": ledger_id,
-                    "ledger_account_id": ledger_account_id,
-                    "effective_at": effective_at,
-                    "effective_date": effective_date,
-                    "posted_at": posted_at,
-                    "updated_at": updated_at,
-                    "status": status,
-                    "external_id": external_id,
-                    "ledger_account_category_id": ledger_account_category_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "ledger_id": ledger_id,
+                        "ledger_account_id": ledger_account_id,
+                        "effective_at": effective_at,
+                        "effective_date": effective_date,
+                        "posted_at": posted_at,
+                        "updated_at": updated_at,
+                        "status": status,
+                        "external_id": external_id,
+                        "ledger_account_category_id": ledger_account_category_id,
+                    },
+                    ledger_transaction_list_params.LedgerTransactionListParams,
+                ),
             ),
             model=LedgerTransaction,
         )
 
 
 class AsyncLedgerTransactions(AsyncAPIResource):
     versions: AsyncVersions
@@ -254,15 +266,15 @@
 
     async def create(
         self,
         *,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         status: Literal["archived", "pending", "posted"] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        effective_date: str,
+        effective_date: Union[str, date],
         ledger_entries: List[ledger_transaction_create_params.LedgerEntry],
         external_id: str | NotGiven = NOT_GIVEN,
         ledgerable_type: Literal[
             "counterparty",
             "expected_payment",
             "incoming_payment_detail",
             "internal_account",
@@ -311,24 +323,27 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/ledger_transactions",
-            body={
-                "description": description,
-                "status": status,
-                "metadata": metadata,
-                "effective_date": effective_date,
-                "ledger_entries": ledger_entries,
-                "external_id": external_id,
-                "ledgerable_type": ledgerable_type,
-                "ledgerable_id": ledgerable_id,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "metadata": metadata,
+                    "effective_date": effective_date,
+                    "ledger_entries": ledger_entries,
+                    "external_id": external_id,
+                    "ledgerable_type": ledgerable_type,
+                    "ledgerable_id": ledgerable_id,
+                },
+                ledger_transaction_create_params.LedgerTransactionCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerTransaction,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -377,36 +392,39 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/ledger_transactions/{id}",
-            body={
-                "description": description,
-                "status": status,
-                "metadata": metadata,
-                "ledger_entries": ledger_entries,
-            },
+            body=maybe_transform(
+                {
+                    "description": description,
+                    "status": status,
+                    "metadata": metadata,
+                    "ledger_entries": ledger_entries,
+                },
+                ledger_transaction_update_params.LedgerTransactionUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LedgerTransaction,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         ledger_id: str | NotGiven = NOT_GIVEN,
         ledger_account_id: str | NotGiven = NOT_GIVEN,
         effective_at: Dict[str, str] | NotGiven = NOT_GIVEN,
-        effective_date: Dict[str, str] | NotGiven = NOT_GIVEN,
-        posted_at: Dict[str, str] | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        effective_date: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
+        posted_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         status: Literal["pending", "posted", "archived"] | NotGiven = NOT_GIVEN,
         external_id: str | NotGiven = NOT_GIVEN,
         ledger_account_category_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
@@ -445,24 +463,27 @@
         return self._get_api_list(
             "/api/ledger_transactions",
             page=AsyncPage[LedgerTransaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "ledger_id": ledger_id,
-                    "ledger_account_id": ledger_account_id,
-                    "effective_at": effective_at,
-                    "effective_date": effective_date,
-                    "posted_at": posted_at,
-                    "updated_at": updated_at,
-                    "status": status,
-                    "external_id": external_id,
-                    "ledger_account_category_id": ledger_account_category_id,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "ledger_id": ledger_id,
+                        "ledger_account_id": ledger_account_id,
+                        "effective_at": effective_at,
+                        "effective_date": effective_date,
+                        "posted_at": posted_at,
+                        "updated_at": updated_at,
+                        "status": status,
+                        "external_id": external_id,
+                        "ledger_account_category_id": ledger_account_category_id,
+                    },
+                    ledger_transaction_list_params.LedgerTransactionListParams,
+                ),
             ),
             model=LedgerTransaction,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledger_transactions/versions.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledger_transactions/versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 import warnings
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import AsyncPaginator, make_request_options
-from ...types.ledger_transactions import LedgerTransactionVersion
+from ...types.ledger_transactions import LedgerTransactionVersion, version_list_params
 
 __all__ = ["Versions", "AsyncVersions"]
 
 
 class Versions(SyncAPIResource):
     def list(
         self,
         id: str,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
-        created_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        created_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         version: Dict[str, int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[LedgerTransactionVersion]:
@@ -49,31 +51,34 @@
         return self._get_api_list(
             f"/api/ledger_transactions/{id}/versions",
             page=SyncPage[LedgerTransactionVersion],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "created_at": created_at,
-                    "version": version,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "created_at": created_at,
+                        "version": version,
+                    },
+                    version_list_params.VersionListParams,
+                ),
             ),
             model=LedgerTransactionVersion,
         )
 
     def versions(
         self,
         id: str,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
-        created_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        created_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         version: Dict[str, int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[LedgerTransactionVersion]:
@@ -110,15 +115,15 @@
 class AsyncVersions(AsyncAPIResource):
     def list(
         self,
         id: str,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
-        created_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        created_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         version: Dict[str, int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[LedgerTransactionVersion, AsyncPage[LedgerTransactionVersion]]:
@@ -142,31 +147,34 @@
         return self._get_api_list(
             f"/api/ledger_transactions/{id}/versions",
             page=AsyncPage[LedgerTransactionVersion],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "created_at": created_at,
-                    "version": version,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "created_at": created_at,
+                        "version": version,
+                    },
+                    version_list_params.VersionListParams,
+                ),
             ),
             model=LedgerTransactionVersion,
         )
 
     def versions(
         self,
         id: str,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
-        created_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        created_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         version: Dict[str, int] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[LedgerTransactionVersion, AsyncPage[LedgerTransactionVersion]]:
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/ledgers.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/ledgers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 
-from ..types import Ledger
+from ..types import (
+    Ledger,
+    ledger_list_params,
+    ledger_create_params,
+    ledger_update_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Ledgers", "AsyncLedgers"]
 
 
@@ -41,19 +48,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/ledgers",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                },
+                ledger_create_params.LedgerCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Ledger,
         )
 
     def retrieve(
         self,
         id: str,
@@ -99,30 +109,33 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/ledgers/{id}",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                },
+                ledger_update_params.LedgerUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Ledger,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[Ledger]:
         """
@@ -146,20 +159,23 @@
         return self._get_api_list(
             "/api/ledgers",
             page=SyncPage[Ledger],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "updated_at": updated_at,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "updated_at": updated_at,
+                    },
+                    ledger_list_params.LedgerListParams,
+                ),
             ),
             model=Ledger,
         )
 
     def delete(
         self,
         id: str,
@@ -206,19 +222,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/ledgers",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                },
+                ledger_create_params.LedgerCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Ledger,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -264,30 +283,33 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/ledgers/{id}",
-            body={
-                "name": name,
-                "description": description,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "metadata": metadata,
+                },
+                ledger_update_params.LedgerUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Ledger,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
-        updated_at: Dict[str, str] | NotGiven = NOT_GIVEN,
+        updated_at: Dict[str, Union[str, datetime]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[Ledger, AsyncPage[Ledger]]:
         """
@@ -311,20 +333,23 @@
         return self._get_api_list(
             "/api/ledgers",
             page=AsyncPage[Ledger],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "metadata": metadata,
-                    "updated_at": updated_at,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "metadata": metadata,
+                        "updated_at": updated_at,
+                    },
+                    ledger_list_params.LedgerListParams,
+                ),
             ),
             model=Ledger,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/line_items.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/line_items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Dict, Optional
 from typing_extensions import Literal
 
-from ..types import LineItem
+from ..types import LineItem, line_item_list_params, line_item_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["LineItems", "AsyncLineItems"]
 
 
@@ -58,15 +59,15 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/{itemizable_type}/{itemizable_id}/line_items/{id}",
-            body={"metadata": metadata},
+            body=maybe_transform({"metadata": metadata}, line_item_update_params.LineItemUpdateParams),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LineItem,
         )
 
     def list(
         self,
         itemizable_id: str,
@@ -93,18 +94,21 @@
         return self._get_api_list(
             f"/api/{itemizable_type}/{itemizable_id}/line_items",
             page=SyncPage[LineItem],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    line_item_list_params.LineItemListParams,
+                ),
             ),
             model=LineItem,
         )
 
 
 class AsyncLineItems(AsyncAPIResource):
     async def retrieve(
@@ -150,15 +154,15 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/{itemizable_type}/{itemizable_id}/line_items/{id}",
-            body={"metadata": metadata},
+            body=maybe_transform({"metadata": metadata}, line_item_update_params.LineItemUpdateParams),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=LineItem,
         )
 
     def list(
         self,
         itemizable_id: str,
@@ -185,14 +189,17 @@
         return self._get_api_list(
             f"/api/{itemizable_type}/{itemizable_id}/line_items",
             page=AsyncPage[LineItem],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    line_item_list_params.LineItemListParams,
+                ),
             ),
             model=LineItem,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/paper_items.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/paper_items.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Union, Optional
+from datetime import date
 
-from ..types import PaperItem
+from ..types import PaperItem, paper_item_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["PaperItems", "AsyncPaperItems"]
 
 
@@ -31,16 +33,16 @@
             cast_to=PaperItem,
         )
 
     def list(
         self,
         *,
         lockbox_number: str | NotGiven = NOT_GIVEN,
-        deposit_date_start: str | NotGiven = NOT_GIVEN,
-        deposit_date_end: str | NotGiven = NOT_GIVEN,
+        deposit_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        deposit_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -65,21 +67,24 @@
         return self._get_api_list(
             "/api/paper_items",
             page=SyncPage[PaperItem],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "lockbox_number": lockbox_number,
-                    "deposit_date_start": deposit_date_start,
-                    "deposit_date_end": deposit_date_end,
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "lockbox_number": lockbox_number,
+                        "deposit_date_start": deposit_date_start,
+                        "deposit_date_end": deposit_date_end,
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    paper_item_list_params.PaperItemListParams,
+                ),
             ),
             model=PaperItem,
         )
 
 
 class AsyncPaperItems(AsyncAPIResource):
     async def retrieve(
@@ -99,16 +104,16 @@
             cast_to=PaperItem,
         )
 
     def list(
         self,
         *,
         lockbox_number: str | NotGiven = NOT_GIVEN,
-        deposit_date_start: str | NotGiven = NOT_GIVEN,
-        deposit_date_end: str | NotGiven = NOT_GIVEN,
+        deposit_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        deposit_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -133,17 +138,20 @@
         return self._get_api_list(
             "/api/paper_items",
             page=AsyncPage[PaperItem],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "lockbox_number": lockbox_number,
-                    "deposit_date_start": deposit_date_start,
-                    "deposit_date_end": deposit_date_end,
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "lockbox_number": lockbox_number,
+                        "deposit_date_start": deposit_date_start,
+                        "deposit_date_end": deposit_date_end,
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    paper_item_list_params.PaperItemListParams,
+                ),
             ),
             model=PaperItem,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/payment_orders/payment_orders.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/payment_orders/payment_orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Dict, List, Mapping, Optional, cast
+from typing import TYPE_CHECKING, Dict, List, Union, Mapping, Optional, cast
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ...types import (
     PaymentOrder,
     PaymentOrderType,
     PaymentOrderSubtype,
     shared,
     shared_params,
+    payment_order_list_params,
     payment_order_create_params,
     payment_order_update_params,
     payment_order_create_async_params,
 )
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
-from ..._utils import extract_files, deepcopy_minimal
+from ..._utils import extract_files, maybe_transform, deepcopy_minimal
 from .reversals import Reversals, AsyncReversals
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import AsyncPaginator, make_request_options
 
 if TYPE_CHECKING:
     from ..._client import ModernTreasury, AsyncModernTreasury
@@ -45,15 +47,15 @@
         priority: Literal["high", "normal"] | NotGiven = NOT_GIVEN,
         originating_account_id: str,
         receiving_account_id: str | NotGiven = NOT_GIVEN,
         accounting: payment_order_create_params.Accounting | NotGiven = NOT_GIVEN,
         accounting_category_id: Optional[str] | NotGiven = NOT_GIVEN,
         accounting_ledger_class_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        effective_date: str | NotGiven = NOT_GIVEN,
+        effective_date: Union[str, date] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         purpose: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         charge_bearer: Optional[Literal["shared", "sender", "receiver"]] | NotGiven = NOT_GIVEN,
         foreign_exchange_indicator: Optional[Literal["fixed_to_variable", "variable_to_fixed"]] | NotGiven = NOT_GIVEN,
@@ -61,15 +63,15 @@
         nsf_protected: bool | NotGiven = NOT_GIVEN,
         originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         send_remittance_advice: Optional[bool] | NotGiven = NOT_GIVEN,
-        expires_at: Optional[str] | NotGiven = NOT_GIVEN,
+        expires_at: Optional[Union[str, datetime]] | NotGiven = NOT_GIVEN,
         fallback_type: Literal["ach"] | NotGiven = NOT_GIVEN,
         receiving_account: payment_order_create_params.ReceivingAccount | NotGiven = NOT_GIVEN,
         ledger_transaction: payment_order_create_params.LedgerTransaction | NotGiven = NOT_GIVEN,
         line_items: List[payment_order_create_params.LineItem] | NotGiven = NOT_GIVEN,
         transaction_monitoring_enabled: bool | NotGiven = NOT_GIVEN,
         documents: List[payment_order_create_params.Document] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -243,15 +245,15 @@
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
 
         return self._post(
             "/api/payment_orders",
-            body=body,
+            body=maybe_transform(body, payment_order_create_params.PaymentOrderCreateParams),
             files=files,
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=PaymentOrder,
         )
 
     def retrieve(
         self,
@@ -281,15 +283,15 @@
         priority: Literal["high", "normal"] | NotGiven = NOT_GIVEN,
         originating_account_id: str | NotGiven = NOT_GIVEN,
         receiving_account_id: str | NotGiven = NOT_GIVEN,
         accounting: payment_order_update_params.Accounting | NotGiven = NOT_GIVEN,
         accounting_category_id: Optional[str] | NotGiven = NOT_GIVEN,
         accounting_ledger_class_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        effective_date: str | NotGiven = NOT_GIVEN,
+        effective_date: Union[str, date] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         purpose: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         charge_bearer: Optional[Literal["shared", "sender", "receiver"]] | NotGiven = NOT_GIVEN,
         foreign_exchange_indicator: Optional[Literal["fixed_to_variable", "variable_to_fixed"]] | NotGiven = NOT_GIVEN,
@@ -297,15 +299,15 @@
         nsf_protected: bool | NotGiven = NOT_GIVEN,
         originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         send_remittance_advice: Optional[bool] | NotGiven = NOT_GIVEN,
-        expires_at: Optional[str] | NotGiven = NOT_GIVEN,
+        expires_at: Optional[Union[str, datetime]] | NotGiven = NOT_GIVEN,
         status: Literal[
             "approved",
             "cancelled",
             "completed",
             "denied",
             "failed",
             "needs_approval",
@@ -449,49 +451,52 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/payment_orders/{id}",
-            body={
-                "type": type,
-                "subtype": subtype,
-                "amount": amount,
-                "direction": direction,
-                "priority": priority,
-                "originating_account_id": originating_account_id,
-                "receiving_account_id": receiving_account_id,
-                "accounting": accounting,
-                "accounting_category_id": accounting_category_id,
-                "accounting_ledger_class_id": accounting_ledger_class_id,
-                "currency": currency,
-                "effective_date": effective_date,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "remittance_information": remittance_information,
-                "purpose": purpose,
-                "metadata": metadata,
-                "charge_bearer": charge_bearer,
-                "foreign_exchange_indicator": foreign_exchange_indicator,
-                "foreign_exchange_contract": foreign_exchange_contract,
-                "nsf_protected": nsf_protected,
-                "originating_party_name": originating_party_name,
-                "ultimate_originating_party_name": ultimate_originating_party_name,
-                "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
-                "ultimate_receiving_party_name": ultimate_receiving_party_name,
-                "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
-                "send_remittance_advice": send_remittance_advice,
-                "expires_at": expires_at,
-                "status": status,
-                "counterparty_id": counterparty_id,
-                "fallback_type": fallback_type,
-                "receiving_account": receiving_account,
-                "line_items": line_items,
-            },
+            body=maybe_transform(
+                {
+                    "type": type,
+                    "subtype": subtype,
+                    "amount": amount,
+                    "direction": direction,
+                    "priority": priority,
+                    "originating_account_id": originating_account_id,
+                    "receiving_account_id": receiving_account_id,
+                    "accounting": accounting,
+                    "accounting_category_id": accounting_category_id,
+                    "accounting_ledger_class_id": accounting_ledger_class_id,
+                    "currency": currency,
+                    "effective_date": effective_date,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "remittance_information": remittance_information,
+                    "purpose": purpose,
+                    "metadata": metadata,
+                    "charge_bearer": charge_bearer,
+                    "foreign_exchange_indicator": foreign_exchange_indicator,
+                    "foreign_exchange_contract": foreign_exchange_contract,
+                    "nsf_protected": nsf_protected,
+                    "originating_party_name": originating_party_name,
+                    "ultimate_originating_party_name": ultimate_originating_party_name,
+                    "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
+                    "ultimate_receiving_party_name": ultimate_receiving_party_name,
+                    "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
+                    "send_remittance_advice": send_remittance_advice,
+                    "expires_at": expires_at,
+                    "status": status,
+                    "counterparty_id": counterparty_id,
+                    "fallback_type": fallback_type,
+                    "receiving_account": receiving_account,
+                    "line_items": line_items,
+                },
+                payment_order_update_params.PaymentOrderUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=PaymentOrder,
         )
 
     def list(
         self,
         *,
@@ -533,16 +538,16 @@
             "returned",
             "reversed",
             "sent",
         ]
         | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         reference_number: str | NotGiven = NOT_GIVEN,
-        effective_date_start: str | NotGiven = NOT_GIVEN,
-        effective_date_end: str | NotGiven = NOT_GIVEN,
+        effective_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        effective_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> SyncPage[PaymentOrder]:
@@ -576,29 +581,32 @@
         return self._get_api_list(
             "/api/payment_orders",
             page=SyncPage[PaymentOrder],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "type": type,
-                    "priority": priority,
-                    "counterparty_id": counterparty_id,
-                    "originating_account_id": originating_account_id,
-                    "transaction_id": transaction_id,
-                    "status": status,
-                    "direction": direction,
-                    "reference_number": reference_number,
-                    "effective_date_start": effective_date_start,
-                    "effective_date_end": effective_date_end,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "type": type,
+                        "priority": priority,
+                        "counterparty_id": counterparty_id,
+                        "originating_account_id": originating_account_id,
+                        "transaction_id": transaction_id,
+                        "status": status,
+                        "direction": direction,
+                        "reference_number": reference_number,
+                        "effective_date_start": effective_date_start,
+                        "effective_date_end": effective_date_end,
+                        "metadata": metadata,
+                    },
+                    payment_order_list_params.PaymentOrderListParams,
+                ),
             ),
             model=PaymentOrder,
         )
 
     def create_async(
         self,
         *,
@@ -609,15 +617,15 @@
         priority: Literal["high", "normal"] | NotGiven = NOT_GIVEN,
         originating_account_id: str,
         receiving_account_id: str | NotGiven = NOT_GIVEN,
         accounting: payment_order_create_async_params.Accounting | NotGiven = NOT_GIVEN,
         accounting_category_id: Optional[str] | NotGiven = NOT_GIVEN,
         accounting_ledger_class_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        effective_date: str | NotGiven = NOT_GIVEN,
+        effective_date: Union[str, date] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         purpose: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         charge_bearer: Optional[Literal["shared", "sender", "receiver"]] | NotGiven = NOT_GIVEN,
         foreign_exchange_indicator: Optional[Literal["fixed_to_variable", "variable_to_fixed"]] | NotGiven = NOT_GIVEN,
@@ -625,15 +633,15 @@
         nsf_protected: bool | NotGiven = NOT_GIVEN,
         originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         send_remittance_advice: Optional[bool] | NotGiven = NOT_GIVEN,
-        expires_at: Optional[str] | NotGiven = NOT_GIVEN,
+        expires_at: Optional[Union[str, datetime]] | NotGiven = NOT_GIVEN,
         fallback_type: Literal["ach"] | NotGiven = NOT_GIVEN,
         receiving_account: payment_order_create_async_params.ReceivingAccount | NotGiven = NOT_GIVEN,
         ledger_transaction: payment_order_create_async_params.LedgerTransaction | NotGiven = NOT_GIVEN,
         line_items: List[payment_order_create_async_params.LineItem] | NotGiven = NOT_GIVEN,
         transaction_monitoring_enabled: bool | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -758,49 +766,52 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/payment_orders/create_async",
-            body={
-                "type": type,
-                "subtype": subtype,
-                "amount": amount,
-                "direction": direction,
-                "priority": priority,
-                "originating_account_id": originating_account_id,
-                "receiving_account_id": receiving_account_id,
-                "accounting": accounting,
-                "accounting_category_id": accounting_category_id,
-                "accounting_ledger_class_id": accounting_ledger_class_id,
-                "currency": currency,
-                "effective_date": effective_date,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "remittance_information": remittance_information,
-                "purpose": purpose,
-                "metadata": metadata,
-                "charge_bearer": charge_bearer,
-                "foreign_exchange_indicator": foreign_exchange_indicator,
-                "foreign_exchange_contract": foreign_exchange_contract,
-                "nsf_protected": nsf_protected,
-                "originating_party_name": originating_party_name,
-                "ultimate_originating_party_name": ultimate_originating_party_name,
-                "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
-                "ultimate_receiving_party_name": ultimate_receiving_party_name,
-                "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
-                "send_remittance_advice": send_remittance_advice,
-                "expires_at": expires_at,
-                "fallback_type": fallback_type,
-                "receiving_account": receiving_account,
-                "ledger_transaction": ledger_transaction,
-                "line_items": line_items,
-                "transaction_monitoring_enabled": transaction_monitoring_enabled,
-            },
+            body=maybe_transform(
+                {
+                    "type": type,
+                    "subtype": subtype,
+                    "amount": amount,
+                    "direction": direction,
+                    "priority": priority,
+                    "originating_account_id": originating_account_id,
+                    "receiving_account_id": receiving_account_id,
+                    "accounting": accounting,
+                    "accounting_category_id": accounting_category_id,
+                    "accounting_ledger_class_id": accounting_ledger_class_id,
+                    "currency": currency,
+                    "effective_date": effective_date,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "remittance_information": remittance_information,
+                    "purpose": purpose,
+                    "metadata": metadata,
+                    "charge_bearer": charge_bearer,
+                    "foreign_exchange_indicator": foreign_exchange_indicator,
+                    "foreign_exchange_contract": foreign_exchange_contract,
+                    "nsf_protected": nsf_protected,
+                    "originating_party_name": originating_party_name,
+                    "ultimate_originating_party_name": ultimate_originating_party_name,
+                    "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
+                    "ultimate_receiving_party_name": ultimate_receiving_party_name,
+                    "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
+                    "send_remittance_advice": send_remittance_advice,
+                    "expires_at": expires_at,
+                    "fallback_type": fallback_type,
+                    "receiving_account": receiving_account,
+                    "ledger_transaction": ledger_transaction,
+                    "line_items": line_items,
+                    "transaction_monitoring_enabled": transaction_monitoring_enabled,
+                },
+                payment_order_create_async_params.PaymentOrderCreateAsyncParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=shared.AsyncResponse,
         )
 
 
 class AsyncPaymentOrders(AsyncAPIResource):
     reversals: AsyncReversals
@@ -819,15 +830,15 @@
         priority: Literal["high", "normal"] | NotGiven = NOT_GIVEN,
         originating_account_id: str,
         receiving_account_id: str | NotGiven = NOT_GIVEN,
         accounting: payment_order_create_params.Accounting | NotGiven = NOT_GIVEN,
         accounting_category_id: Optional[str] | NotGiven = NOT_GIVEN,
         accounting_ledger_class_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        effective_date: str | NotGiven = NOT_GIVEN,
+        effective_date: Union[str, date] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         purpose: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         charge_bearer: Optional[Literal["shared", "sender", "receiver"]] | NotGiven = NOT_GIVEN,
         foreign_exchange_indicator: Optional[Literal["fixed_to_variable", "variable_to_fixed"]] | NotGiven = NOT_GIVEN,
@@ -835,15 +846,15 @@
         nsf_protected: bool | NotGiven = NOT_GIVEN,
         originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         send_remittance_advice: Optional[bool] | NotGiven = NOT_GIVEN,
-        expires_at: Optional[str] | NotGiven = NOT_GIVEN,
+        expires_at: Optional[Union[str, datetime]] | NotGiven = NOT_GIVEN,
         fallback_type: Literal["ach"] | NotGiven = NOT_GIVEN,
         receiving_account: payment_order_create_params.ReceivingAccount | NotGiven = NOT_GIVEN,
         ledger_transaction: payment_order_create_params.LedgerTransaction | NotGiven = NOT_GIVEN,
         line_items: List[payment_order_create_params.LineItem] | NotGiven = NOT_GIVEN,
         transaction_monitoring_enabled: bool | NotGiven = NOT_GIVEN,
         documents: List[payment_order_create_params.Document] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -1017,15 +1028,15 @@
             # It should be noted that the actual Content-Type header that will be
             # sent to the server will contain a `boundary` parameter, e.g.
             # multipart/form-data; boundary=---abc--
             extra_headers = {"Content-Type": "multipart/form-data", **(extra_headers or {})}
 
         return await self._post(
             "/api/payment_orders",
-            body=body,
+            body=maybe_transform(body, payment_order_create_params.PaymentOrderCreateParams),
             files=files,
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=PaymentOrder,
         )
 
     async def retrieve(
         self,
@@ -1055,15 +1066,15 @@
         priority: Literal["high", "normal"] | NotGiven = NOT_GIVEN,
         originating_account_id: str | NotGiven = NOT_GIVEN,
         receiving_account_id: str | NotGiven = NOT_GIVEN,
         accounting: payment_order_update_params.Accounting | NotGiven = NOT_GIVEN,
         accounting_category_id: Optional[str] | NotGiven = NOT_GIVEN,
         accounting_ledger_class_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        effective_date: str | NotGiven = NOT_GIVEN,
+        effective_date: Union[str, date] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         purpose: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         charge_bearer: Optional[Literal["shared", "sender", "receiver"]] | NotGiven = NOT_GIVEN,
         foreign_exchange_indicator: Optional[Literal["fixed_to_variable", "variable_to_fixed"]] | NotGiven = NOT_GIVEN,
@@ -1071,15 +1082,15 @@
         nsf_protected: bool | NotGiven = NOT_GIVEN,
         originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         send_remittance_advice: Optional[bool] | NotGiven = NOT_GIVEN,
-        expires_at: Optional[str] | NotGiven = NOT_GIVEN,
+        expires_at: Optional[Union[str, datetime]] | NotGiven = NOT_GIVEN,
         status: Literal[
             "approved",
             "cancelled",
             "completed",
             "denied",
             "failed",
             "needs_approval",
@@ -1223,49 +1234,52 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/payment_orders/{id}",
-            body={
-                "type": type,
-                "subtype": subtype,
-                "amount": amount,
-                "direction": direction,
-                "priority": priority,
-                "originating_account_id": originating_account_id,
-                "receiving_account_id": receiving_account_id,
-                "accounting": accounting,
-                "accounting_category_id": accounting_category_id,
-                "accounting_ledger_class_id": accounting_ledger_class_id,
-                "currency": currency,
-                "effective_date": effective_date,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "remittance_information": remittance_information,
-                "purpose": purpose,
-                "metadata": metadata,
-                "charge_bearer": charge_bearer,
-                "foreign_exchange_indicator": foreign_exchange_indicator,
-                "foreign_exchange_contract": foreign_exchange_contract,
-                "nsf_protected": nsf_protected,
-                "originating_party_name": originating_party_name,
-                "ultimate_originating_party_name": ultimate_originating_party_name,
-                "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
-                "ultimate_receiving_party_name": ultimate_receiving_party_name,
-                "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
-                "send_remittance_advice": send_remittance_advice,
-                "expires_at": expires_at,
-                "status": status,
-                "counterparty_id": counterparty_id,
-                "fallback_type": fallback_type,
-                "receiving_account": receiving_account,
-                "line_items": line_items,
-            },
+            body=maybe_transform(
+                {
+                    "type": type,
+                    "subtype": subtype,
+                    "amount": amount,
+                    "direction": direction,
+                    "priority": priority,
+                    "originating_account_id": originating_account_id,
+                    "receiving_account_id": receiving_account_id,
+                    "accounting": accounting,
+                    "accounting_category_id": accounting_category_id,
+                    "accounting_ledger_class_id": accounting_ledger_class_id,
+                    "currency": currency,
+                    "effective_date": effective_date,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "remittance_information": remittance_information,
+                    "purpose": purpose,
+                    "metadata": metadata,
+                    "charge_bearer": charge_bearer,
+                    "foreign_exchange_indicator": foreign_exchange_indicator,
+                    "foreign_exchange_contract": foreign_exchange_contract,
+                    "nsf_protected": nsf_protected,
+                    "originating_party_name": originating_party_name,
+                    "ultimate_originating_party_name": ultimate_originating_party_name,
+                    "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
+                    "ultimate_receiving_party_name": ultimate_receiving_party_name,
+                    "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
+                    "send_remittance_advice": send_remittance_advice,
+                    "expires_at": expires_at,
+                    "status": status,
+                    "counterparty_id": counterparty_id,
+                    "fallback_type": fallback_type,
+                    "receiving_account": receiving_account,
+                    "line_items": line_items,
+                },
+                payment_order_update_params.PaymentOrderUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=PaymentOrder,
         )
 
     def list(
         self,
         *,
@@ -1307,16 +1321,16 @@
             "returned",
             "reversed",
             "sent",
         ]
         | NotGiven = NOT_GIVEN,
         direction: Literal["credit", "debit"] | NotGiven = NOT_GIVEN,
         reference_number: str | NotGiven = NOT_GIVEN,
-        effective_date_start: str | NotGiven = NOT_GIVEN,
-        effective_date_end: str | NotGiven = NOT_GIVEN,
+        effective_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        effective_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
     ) -> AsyncPaginator[PaymentOrder, AsyncPage[PaymentOrder]]:
@@ -1350,29 +1364,32 @@
         return self._get_api_list(
             "/api/payment_orders",
             page=AsyncPage[PaymentOrder],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "type": type,
-                    "priority": priority,
-                    "counterparty_id": counterparty_id,
-                    "originating_account_id": originating_account_id,
-                    "transaction_id": transaction_id,
-                    "status": status,
-                    "direction": direction,
-                    "reference_number": reference_number,
-                    "effective_date_start": effective_date_start,
-                    "effective_date_end": effective_date_end,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "type": type,
+                        "priority": priority,
+                        "counterparty_id": counterparty_id,
+                        "originating_account_id": originating_account_id,
+                        "transaction_id": transaction_id,
+                        "status": status,
+                        "direction": direction,
+                        "reference_number": reference_number,
+                        "effective_date_start": effective_date_start,
+                        "effective_date_end": effective_date_end,
+                        "metadata": metadata,
+                    },
+                    payment_order_list_params.PaymentOrderListParams,
+                ),
             ),
             model=PaymentOrder,
         )
 
     async def create_async(
         self,
         *,
@@ -1383,15 +1400,15 @@
         priority: Literal["high", "normal"] | NotGiven = NOT_GIVEN,
         originating_account_id: str,
         receiving_account_id: str | NotGiven = NOT_GIVEN,
         accounting: payment_order_create_async_params.Accounting | NotGiven = NOT_GIVEN,
         accounting_category_id: Optional[str] | NotGiven = NOT_GIVEN,
         accounting_ledger_class_id: Optional[str] | NotGiven = NOT_GIVEN,
         currency: shared_params.Currency | NotGiven = NOT_GIVEN,
-        effective_date: str | NotGiven = NOT_GIVEN,
+        effective_date: Union[str, date] | NotGiven = NOT_GIVEN,
         description: Optional[str] | NotGiven = NOT_GIVEN,
         statement_descriptor: Optional[str] | NotGiven = NOT_GIVEN,
         remittance_information: Optional[str] | NotGiven = NOT_GIVEN,
         purpose: Optional[str] | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         charge_bearer: Optional[Literal["shared", "sender", "receiver"]] | NotGiven = NOT_GIVEN,
         foreign_exchange_indicator: Optional[Literal["fixed_to_variable", "variable_to_fixed"]] | NotGiven = NOT_GIVEN,
@@ -1399,15 +1416,15 @@
         nsf_protected: bool | NotGiven = NOT_GIVEN,
         originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_originating_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_name: Optional[str] | NotGiven = NOT_GIVEN,
         ultimate_receiving_party_identifier: Optional[str] | NotGiven = NOT_GIVEN,
         send_remittance_advice: Optional[bool] | NotGiven = NOT_GIVEN,
-        expires_at: Optional[str] | NotGiven = NOT_GIVEN,
+        expires_at: Optional[Union[str, datetime]] | NotGiven = NOT_GIVEN,
         fallback_type: Literal["ach"] | NotGiven = NOT_GIVEN,
         receiving_account: payment_order_create_async_params.ReceivingAccount | NotGiven = NOT_GIVEN,
         ledger_transaction: payment_order_create_async_params.LedgerTransaction | NotGiven = NOT_GIVEN,
         line_items: List[payment_order_create_async_params.LineItem] | NotGiven = NOT_GIVEN,
         transaction_monitoring_enabled: bool | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
@@ -1532,45 +1549,48 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/payment_orders/create_async",
-            body={
-                "type": type,
-                "subtype": subtype,
-                "amount": amount,
-                "direction": direction,
-                "priority": priority,
-                "originating_account_id": originating_account_id,
-                "receiving_account_id": receiving_account_id,
-                "accounting": accounting,
-                "accounting_category_id": accounting_category_id,
-                "accounting_ledger_class_id": accounting_ledger_class_id,
-                "currency": currency,
-                "effective_date": effective_date,
-                "description": description,
-                "statement_descriptor": statement_descriptor,
-                "remittance_information": remittance_information,
-                "purpose": purpose,
-                "metadata": metadata,
-                "charge_bearer": charge_bearer,
-                "foreign_exchange_indicator": foreign_exchange_indicator,
-                "foreign_exchange_contract": foreign_exchange_contract,
-                "nsf_protected": nsf_protected,
-                "originating_party_name": originating_party_name,
-                "ultimate_originating_party_name": ultimate_originating_party_name,
-                "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
-                "ultimate_receiving_party_name": ultimate_receiving_party_name,
-                "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
-                "send_remittance_advice": send_remittance_advice,
-                "expires_at": expires_at,
-                "fallback_type": fallback_type,
-                "receiving_account": receiving_account,
-                "ledger_transaction": ledger_transaction,
-                "line_items": line_items,
-                "transaction_monitoring_enabled": transaction_monitoring_enabled,
-            },
+            body=maybe_transform(
+                {
+                    "type": type,
+                    "subtype": subtype,
+                    "amount": amount,
+                    "direction": direction,
+                    "priority": priority,
+                    "originating_account_id": originating_account_id,
+                    "receiving_account_id": receiving_account_id,
+                    "accounting": accounting,
+                    "accounting_category_id": accounting_category_id,
+                    "accounting_ledger_class_id": accounting_ledger_class_id,
+                    "currency": currency,
+                    "effective_date": effective_date,
+                    "description": description,
+                    "statement_descriptor": statement_descriptor,
+                    "remittance_information": remittance_information,
+                    "purpose": purpose,
+                    "metadata": metadata,
+                    "charge_bearer": charge_bearer,
+                    "foreign_exchange_indicator": foreign_exchange_indicator,
+                    "foreign_exchange_contract": foreign_exchange_contract,
+                    "nsf_protected": nsf_protected,
+                    "originating_party_name": originating_party_name,
+                    "ultimate_originating_party_name": ultimate_originating_party_name,
+                    "ultimate_originating_party_identifier": ultimate_originating_party_identifier,
+                    "ultimate_receiving_party_name": ultimate_receiving_party_name,
+                    "ultimate_receiving_party_identifier": ultimate_receiving_party_identifier,
+                    "send_remittance_advice": send_remittance_advice,
+                    "expires_at": expires_at,
+                    "fallback_type": fallback_type,
+                    "receiving_account": receiving_account,
+                    "ledger_transaction": ledger_transaction,
+                    "line_items": line_items,
+                    "transaction_monitoring_enabled": transaction_monitoring_enabled,
+                },
+                payment_order_create_async_params.PaymentOrderCreateAsyncParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=shared.AsyncResponse,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/payment_orders/reversals.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/payment_orders/reversals.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,23 @@
 
 from __future__ import annotations
 
 from typing import Dict, Optional
 from typing_extensions import Literal
 
 from ..._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from ..._utils import maybe_transform
 from ..._resource import SyncAPIResource, AsyncAPIResource
 from ...pagination import SyncPage, AsyncPage
 from ..._base_client import AsyncPaginator, make_request_options
-from ...types.payment_orders import Reversal, reversal_create_params
+from ...types.payment_orders import (
+    Reversal,
+    reversal_list_params,
+    reversal_create_params,
+)
 
 __all__ = ["Reversals", "AsyncReversals"]
 
 
 class Reversals(SyncAPIResource):
     def create(
         self,
@@ -53,19 +58,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             f"/api/payment_orders/{payment_order_id}/reversals",
-            body={
-                "reason": reason,
-                "metadata": metadata,
-                "ledger_transaction": ledger_transaction,
-            },
+            body=maybe_transform(
+                {
+                    "reason": reason,
+                    "metadata": metadata,
+                    "ledger_transaction": ledger_transaction,
+                },
+                reversal_create_params.ReversalCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Reversal,
         )
 
     def retrieve(
         self,
         reversal_id: str,
@@ -109,18 +117,21 @@
         return self._get_api_list(
             f"/api/payment_orders/{payment_order_id}/reversals",
             page=SyncPage[Reversal],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    reversal_list_params.ReversalListParams,
+                ),
             ),
             model=Reversal,
         )
 
 
 class AsyncReversals(AsyncAPIResource):
     async def create(
@@ -161,19 +172,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             f"/api/payment_orders/{payment_order_id}/reversals",
-            body={
-                "reason": reason,
-                "metadata": metadata,
-                "ledger_transaction": ledger_transaction,
-            },
+            body=maybe_transform(
+                {
+                    "reason": reason,
+                    "metadata": metadata,
+                    "ledger_transaction": ledger_transaction,
+                },
+                reversal_create_params.ReversalCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Reversal,
         )
 
     async def retrieve(
         self,
         reversal_id: str,
@@ -217,14 +231,17 @@
         return self._get_api_list(
             f"/api/payment_orders/{payment_order_id}/reversals",
             page=AsyncPage[Reversal],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    reversal_list_params.ReversalListParams,
+                ),
             ),
             model=Reversal,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/payment_references.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/payment_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Optional
 from typing_extensions import Literal
 
-from ..types import PaymentReference
+from ..types import PaymentReference, payment_reference_list_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["PaymentReferences", "AsyncPaymentReferences"]
 
 
@@ -50,21 +51,24 @@
         return self._get_api_list(
             "/api/payment_references",
             page=SyncPage[PaymentReference],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "referenceable_id": referenceable_id,
-                    "referenceable_type": referenceable_type,
-                    "reference_number": reference_number,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "referenceable_id": referenceable_id,
+                        "referenceable_type": referenceable_type,
+                        "reference_number": reference_number,
+                    },
+                    payment_reference_list_params.PaymentReferenceListParams,
+                ),
             ),
             model=PaymentReference,
         )
 
     def retireve(
         self,
         id: str,
@@ -119,21 +123,24 @@
         return self._get_api_list(
             "/api/payment_references",
             page=AsyncPage[PaymentReference],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "referenceable_id": referenceable_id,
-                    "referenceable_type": referenceable_type,
-                    "reference_number": reference_number,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "referenceable_id": referenceable_id,
+                        "referenceable_type": referenceable_type,
+                        "reference_number": reference_number,
+                    },
+                    payment_reference_list_params.PaymentReferenceListParams,
+                ),
             ),
             model=PaymentReference,
         )
 
     async def retireve(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/returns.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/returns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Union, Optional
+from datetime import date
 from typing_extensions import Literal
 
-from ..types import ReturnObject
+from ..types import ReturnObject, return_list_params, return_create_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Returns", "AsyncReturns"]
 
 
@@ -64,15 +66,15 @@
                 "R52",
                 "R53",
                 "currencycloud",
             ]
         ]
         | NotGiven = NOT_GIVEN,
         reason: Optional[str] | NotGiven = NOT_GIVEN,
-        date_of_death: Optional[str] | NotGiven = NOT_GIVEN,
+        date_of_death: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         additional_information: Optional[str] | NotGiven = NOT_GIVEN,
         returnable_type: Literal["incoming_payment_detail"],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -101,22 +103,25 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/returns",
-            body={
-                "returnable_id": returnable_id,
-                "code": code,
-                "reason": reason,
-                "date_of_death": date_of_death,
-                "additional_information": additional_information,
-                "returnable_type": returnable_type,
-            },
+            body=maybe_transform(
+                {
+                    "returnable_id": returnable_id,
+                    "code": code,
+                    "reason": reason,
+                    "date_of_death": date_of_death,
+                    "additional_information": additional_information,
+                    "returnable_type": returnable_type,
+                },
+                return_create_params.ReturnCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ReturnObject,
         )
 
     def retrieve(
         self,
         id: str,
@@ -174,22 +179,25 @@
         return self._get_api_list(
             "/api/returns",
             page=SyncPage[ReturnObject],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "internal_account_id": internal_account_id,
-                    "counterparty_id": counterparty_id,
-                    "returnable_id": returnable_id,
-                    "returnable_type": returnable_type,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "internal_account_id": internal_account_id,
+                        "counterparty_id": counterparty_id,
+                        "returnable_id": returnable_id,
+                        "returnable_type": returnable_type,
+                    },
+                    return_list_params.ReturnListParams,
+                ),
             ),
             model=ReturnObject,
         )
 
 
 class AsyncReturns(AsyncAPIResource):
     async def create(
@@ -241,15 +249,15 @@
                 "R52",
                 "R53",
                 "currencycloud",
             ]
         ]
         | NotGiven = NOT_GIVEN,
         reason: Optional[str] | NotGiven = NOT_GIVEN,
-        date_of_death: Optional[str] | NotGiven = NOT_GIVEN,
+        date_of_death: Optional[Union[str, date]] | NotGiven = NOT_GIVEN,
         additional_information: Optional[str] | NotGiven = NOT_GIVEN,
         returnable_type: Literal["incoming_payment_detail"],
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
@@ -278,22 +286,25 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/returns",
-            body={
-                "returnable_id": returnable_id,
-                "code": code,
-                "reason": reason,
-                "date_of_death": date_of_death,
-                "additional_information": additional_information,
-                "returnable_type": returnable_type,
-            },
+            body=maybe_transform(
+                {
+                    "returnable_id": returnable_id,
+                    "code": code,
+                    "reason": reason,
+                    "date_of_death": date_of_death,
+                    "additional_information": additional_information,
+                    "returnable_type": returnable_type,
+                },
+                return_create_params.ReturnCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=ReturnObject,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -351,18 +362,21 @@
         return self._get_api_list(
             "/api/returns",
             page=AsyncPage[ReturnObject],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "internal_account_id": internal_account_id,
-                    "counterparty_id": counterparty_id,
-                    "returnable_id": returnable_id,
-                    "returnable_type": returnable_type,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "internal_account_id": internal_account_id,
+                        "counterparty_id": counterparty_id,
+                        "returnable_id": returnable_id,
+                        "returnable_type": returnable_type,
+                    },
+                    return_list_params.ReturnListParams,
+                ),
             ),
             model=ReturnObject,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/routing_details.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/routing_details.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Optional
 from typing_extensions import Literal
 
-from ..types import RoutingDetail
+from ..types import (
+    RoutingDetail,
+    routing_detail_list_params,
+    routing_detail_create_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["RoutingDetails", "AsyncRoutingDetails"]
 
 
@@ -67,19 +72,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             f"/api/{accounts_type}/{account_id}/routing_details",
-            body={
-                "routing_number": routing_number,
-                "routing_number_type": routing_number_type,
-                "payment_type": payment_type,
-            },
+            body=maybe_transform(
+                {
+                    "routing_number": routing_number,
+                    "routing_number_type": routing_number_type,
+                    "payment_type": payment_type,
+                },
+                routing_detail_create_params.RoutingDetailCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=RoutingDetail,
         )
 
     def retrieve(
         self,
         id: str,
@@ -125,18 +133,21 @@
         return self._get_api_list(
             f"/api/{accounts_type}/{account_id}/routing_details",
             page=SyncPage[RoutingDetail],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    routing_detail_list_params.RoutingDetailListParams,
+                ),
             ),
             model=RoutingDetail,
         )
 
     def delete(
         self,
         id: str,
@@ -211,19 +222,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             f"/api/{accounts_type}/{account_id}/routing_details",
-            body={
-                "routing_number": routing_number,
-                "routing_number_type": routing_number_type,
-                "payment_type": payment_type,
-            },
+            body=maybe_transform(
+                {
+                    "routing_number": routing_number,
+                    "routing_number_type": routing_number_type,
+                    "payment_type": payment_type,
+                },
+                routing_detail_create_params.RoutingDetailCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=RoutingDetail,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -269,18 +283,21 @@
         return self._get_api_list(
             f"/api/{accounts_type}/{account_id}/routing_details",
             page=AsyncPage[RoutingDetail],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                    },
+                    routing_detail_list_params.RoutingDetailListParams,
+                ),
             ),
             model=RoutingDetail,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/transactions.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/transactions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import date
 
-from ..types import Transaction
+from ..types import Transaction, transaction_list_params, transaction_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["Transactions", "AsyncTransactions"]
 
 
@@ -53,29 +55,29 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/transactions/{id}",
-            body={"metadata": metadata},
+            body=maybe_transform({"metadata": metadata}, transaction_update_params.TransactionUpdateParams),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Transaction,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         internal_account_id: str | NotGiven = NOT_GIVEN,
         virtual_account_id: str | NotGiven = NOT_GIVEN,
         posted: bool | NotGiven = NOT_GIVEN,
-        as_of_date_start: str | NotGiven = NOT_GIVEN,
-        as_of_date_end: str | NotGiven = NOT_GIVEN,
+        as_of_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        as_of_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         direction: str | NotGiven = NOT_GIVEN,
         counterparty_id: str | NotGiven = NOT_GIVEN,
         payment_type: str | NotGiven = NOT_GIVEN,
         transactable_type: str | NotGiven = NOT_GIVEN,
         description: str | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -114,29 +116,32 @@
         return self._get_api_list(
             "/api/transactions",
             page=SyncPage[Transaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "internal_account_id": internal_account_id,
-                    "virtual_account_id": virtual_account_id,
-                    "posted": posted,
-                    "as_of_date_start": as_of_date_start,
-                    "as_of_date_end": as_of_date_end,
-                    "direction": direction,
-                    "counterparty_id": counterparty_id,
-                    "payment_type": payment_type,
-                    "transactable_type": transactable_type,
-                    "description": description,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "internal_account_id": internal_account_id,
+                        "virtual_account_id": virtual_account_id,
+                        "posted": posted,
+                        "as_of_date_start": as_of_date_start,
+                        "as_of_date_end": as_of_date_end,
+                        "direction": direction,
+                        "counterparty_id": counterparty_id,
+                        "payment_type": payment_type,
+                        "transactable_type": transactable_type,
+                        "description": description,
+                        "metadata": metadata,
+                    },
+                    transaction_list_params.TransactionListParams,
+                ),
             ),
             model=Transaction,
         )
 
 
 class AsyncTransactions(AsyncAPIResource):
     async def retrieve(
@@ -178,29 +183,29 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/transactions/{id}",
-            body={"metadata": metadata},
+            body=maybe_transform({"metadata": metadata}, transaction_update_params.TransactionUpdateParams),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=Transaction,
         )
 
     def list(
         self,
         *,
         after_cursor: Optional[str] | NotGiven = NOT_GIVEN,
         per_page: int | NotGiven = NOT_GIVEN,
         internal_account_id: str | NotGiven = NOT_GIVEN,
         virtual_account_id: str | NotGiven = NOT_GIVEN,
         posted: bool | NotGiven = NOT_GIVEN,
-        as_of_date_start: str | NotGiven = NOT_GIVEN,
-        as_of_date_end: str | NotGiven = NOT_GIVEN,
+        as_of_date_start: Union[str, date] | NotGiven = NOT_GIVEN,
+        as_of_date_end: Union[str, date] | NotGiven = NOT_GIVEN,
         direction: str | NotGiven = NOT_GIVEN,
         counterparty_id: str | NotGiven = NOT_GIVEN,
         payment_type: str | NotGiven = NOT_GIVEN,
         transactable_type: str | NotGiven = NOT_GIVEN,
         description: str | NotGiven = NOT_GIVEN,
         metadata: Dict[str, str] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
@@ -239,25 +244,28 @@
         return self._get_api_list(
             "/api/transactions",
             page=AsyncPage[Transaction],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "internal_account_id": internal_account_id,
-                    "virtual_account_id": virtual_account_id,
-                    "posted": posted,
-                    "as_of_date_start": as_of_date_start,
-                    "as_of_date_end": as_of_date_end,
-                    "direction": direction,
-                    "counterparty_id": counterparty_id,
-                    "payment_type": payment_type,
-                    "transactable_type": transactable_type,
-                    "description": description,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "internal_account_id": internal_account_id,
+                        "virtual_account_id": virtual_account_id,
+                        "posted": posted,
+                        "as_of_date_start": as_of_date_start,
+                        "as_of_date_end": as_of_date_end,
+                        "direction": direction,
+                        "counterparty_id": counterparty_id,
+                        "payment_type": payment_type,
+                        "transactable_type": transactable_type,
+                        "description": description,
+                        "metadata": metadata,
+                    },
+                    transaction_list_params.TransactionListParams,
+                ),
             ),
             model=Transaction,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/validations.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/validations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing_extensions import Literal
 
-from ..types import RoutingNumberLookupRequest
+from ..types import (
+    RoutingNumberLookupRequest,
+    validation_validate_routing_number_params,
+)
 from .._types import Body, Query, Headers
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from .._base_client import make_request_options
 
 __all__ = ["Validations", "AsyncValidations"]
 
 
 class Validations(SyncAPIResource):
@@ -46,18 +50,21 @@
         """
         return self._get(
             "/api/validations/routing_numbers",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "routing_number": routing_number,
-                    "routing_number_type": routing_number_type,
-                },
+                query=maybe_transform(
+                    {
+                        "routing_number": routing_number,
+                        "routing_number_type": routing_number_type,
+                    },
+                    validation_validate_routing_number_params.ValidationValidateRoutingNumberParams,
+                ),
             ),
             cast_to=RoutingNumberLookupRequest,
         )
 
 
 class AsyncValidations(AsyncAPIResource):
     async def validate_routing_number(
@@ -93,14 +100,17 @@
         """
         return await self._get(
             "/api/validations/routing_numbers",
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "routing_number": routing_number,
-                    "routing_number_type": routing_number_type,
-                },
+                query=maybe_transform(
+                    {
+                        "routing_number": routing_number,
+                        "routing_number_type": routing_number_type,
+                    },
+                    validation_validate_routing_number_params.ValidationValidateRoutingNumberParams,
+                ),
             ),
             cast_to=RoutingNumberLookupRequest,
         )
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/virtual_accounts.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/virtual_accounts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
 from typing import Dict, List, Optional
 
-from ..types import VirtualAccount, virtual_account_create_params
+from ..types import (
+    VirtualAccount,
+    virtual_account_list_params,
+    virtual_account_create_params,
+    virtual_account_update_params,
+)
 from .._types import NOT_GIVEN, Body, Query, Headers, NoneType, NotGiven
+from .._utils import maybe_transform
 from .._resource import SyncAPIResource, AsyncAPIResource
 from ..pagination import SyncPage, AsyncPage
 from .._base_client import AsyncPaginator, make_request_options
 
 __all__ = ["VirtualAccounts", "AsyncVirtualAccounts"]
 
 
@@ -63,25 +69,28 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._post(
             "/api/virtual_accounts",
-            body={
-                "name": name,
-                "description": description,
-                "counterparty_id": counterparty_id,
-                "internal_account_id": internal_account_id,
-                "account_details": account_details,
-                "routing_details": routing_details,
-                "debit_ledger_account_id": debit_ledger_account_id,
-                "credit_ledger_account_id": credit_ledger_account_id,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "counterparty_id": counterparty_id,
+                    "internal_account_id": internal_account_id,
+                    "account_details": account_details,
+                    "routing_details": routing_details,
+                    "debit_ledger_account_id": debit_ledger_account_id,
+                    "credit_ledger_account_id": credit_ledger_account_id,
+                    "metadata": metadata,
+                },
+                virtual_account_create_params.VirtualAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=VirtualAccount,
         )
 
     def retrieve(
         self,
         id: str,
@@ -121,19 +130,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return self._patch(
             f"/api/virtual_accounts/{id}",
-            body={
-                "name": name,
-                "counterparty_id": counterparty_id,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "counterparty_id": counterparty_id,
+                    "metadata": metadata,
+                },
+                virtual_account_update_params.VirtualAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=VirtualAccount,
         )
 
     def list(
         self,
         *,
@@ -165,21 +177,24 @@
         return self._get_api_list(
             "/api/virtual_accounts",
             page=SyncPage[VirtualAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "internal_account_id": internal_account_id,
-                    "counterparty_id": counterparty_id,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "internal_account_id": internal_account_id,
+                        "counterparty_id": counterparty_id,
+                        "metadata": metadata,
+                    },
+                    virtual_account_list_params.VirtualAccountListParams,
+                ),
             ),
             model=VirtualAccount,
         )
 
     def delete(
         self,
         id: str,
@@ -248,25 +263,28 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._post(
             "/api/virtual_accounts",
-            body={
-                "name": name,
-                "description": description,
-                "counterparty_id": counterparty_id,
-                "internal_account_id": internal_account_id,
-                "account_details": account_details,
-                "routing_details": routing_details,
-                "debit_ledger_account_id": debit_ledger_account_id,
-                "credit_ledger_account_id": credit_ledger_account_id,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "description": description,
+                    "counterparty_id": counterparty_id,
+                    "internal_account_id": internal_account_id,
+                    "account_details": account_details,
+                    "routing_details": routing_details,
+                    "debit_ledger_account_id": debit_ledger_account_id,
+                    "credit_ledger_account_id": credit_ledger_account_id,
+                    "metadata": metadata,
+                },
+                virtual_account_create_params.VirtualAccountCreateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=VirtualAccount,
         )
 
     async def retrieve(
         self,
         id: str,
@@ -306,19 +324,22 @@
 
           extra_query: Add additional query parameters to the request
 
           extra_body: Add additional JSON properties to the request
         """
         return await self._patch(
             f"/api/virtual_accounts/{id}",
-            body={
-                "name": name,
-                "counterparty_id": counterparty_id,
-                "metadata": metadata,
-            },
+            body=maybe_transform(
+                {
+                    "name": name,
+                    "counterparty_id": counterparty_id,
+                    "metadata": metadata,
+                },
+                virtual_account_update_params.VirtualAccountUpdateParams,
+            ),
             options=make_request_options(extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body),
             cast_to=VirtualAccount,
         )
 
     def list(
         self,
         *,
@@ -350,21 +371,24 @@
         return self._get_api_list(
             "/api/virtual_accounts",
             page=AsyncPage[VirtualAccount],
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
                 extra_body=extra_body,
-                query={
-                    "after_cursor": after_cursor,
-                    "per_page": per_page,
-                    "internal_account_id": internal_account_id,
-                    "counterparty_id": counterparty_id,
-                    "metadata": metadata,
-                },
+                query=maybe_transform(
+                    {
+                        "after_cursor": after_cursor,
+                        "per_page": per_page,
+                        "internal_account_id": internal_account_id,
+                        "counterparty_id": counterparty_id,
+                        "metadata": metadata,
+                    },
+                    virtual_account_list_params.VirtualAccountListParams,
+                ),
             ),
             model=VirtualAccount,
         )
 
     async def delete(
         self,
         id: str,
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/resources/webhooks.py` & `modern_treasury-1.9.0/src/modern_treasury/resources/webhooks.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/__init__.py` & `modern_treasury-1.9.0/src/modern_treasury/types/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/account_detail.py` & `modern_treasury-1.9.0/src/modern_treasury/types/account_detail.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["AccountDetail"]
 
 
@@ -14,25 +15,25 @@
 
     account_number_type: Literal["clabe", "iban", "other", "pan", "wallet_address"]
     """One of `iban`, `clabe`, `wallet_address`, or `other`.
 
     Use `other` if the bank account number is in a generic format.
     """
 
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
 
     account_number: Optional[str]
     """The account number for the bank account."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/account_detail_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/account_detail_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/connection.py` & `modern_treasury-1.9.0/src/modern_treasury/types/connection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
+from datetime import datetime
 
 from .._models import BaseModel
 
 __all__ = ["Connection"]
 
 
 class Connection(BaseModel):
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
 
     vendor_customer_id: Optional[str]
     """An identifier given to this connection by the bank."""
 
     vendor_id: str
     """Unique identifier for the bank or vendor."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/counterparty.py` & `modern_treasury-1.9.0/src/modern_treasury/types/counterparty.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from ..types import account_detail, routing_detail, external_account_type
 from .._models import BaseModel
 
 __all__ = [
     "Counterparty",
@@ -17,15 +18,15 @@
 ]
 
 
 class AccountPartyAddress(BaseModel):
     country: Optional[str]
     """Country code conforms to [ISO 3166-1 alpha-2]"""
 
-    created_at: str
+    created_at: datetime
 
     id: str
 
     line1: Optional[str]
 
     line2: Optional[str]
 
@@ -42,44 +43,44 @@
 
     postal_code: Optional[str]
     """The postal code of the address."""
 
     region: Optional[str]
     """Region or State."""
 
-    updated_at: str
+    updated_at: datetime
 
 
 AccountsPartyAddress = AccountPartyAddress
 """This type is deprecated and will be removed in a future release.
 
 Please use AccountPartyAddress instead.
 """
 
 
 class AccountContactDetail(BaseModel):
     contact_identifier: str
 
     contact_identifier_type: Literal["email", "phone_number", "website"]
 
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
 
 
 AccountsContactDetails = AccountContactDetail
 """This type is deprecated and will be removed in a future release.
 
 Please use AccountContactDetail instead.
 """
@@ -89,17 +90,17 @@
     account_details: Optional[List[account_detail.AccountDetail]]
 
     account_type: Optional[external_account_type.ExternalAccountType]
     """Can be `checking`, `savings` or `other`."""
 
     contact_details: Optional[List[AccountContactDetail]]
 
-    created_at: Optional[str]
+    created_at: Optional[datetime]
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: Optional[str]
 
     live_mode: Optional[bool]
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -126,15 +127,15 @@
     """The legal name of the entity which owns the account."""
 
     party_type: Optional[Literal["business", "individual"]]
     """Either `individual` or `business`."""
 
     routing_details: Optional[List[routing_detail.RoutingDetail]]
 
-    updated_at: Optional[str]
+    updated_at: Optional[datetime]
 
     verification_status: Optional[Literal["pending_verification", "unverified", "verified"]]
 
 
 Accounts = Account
 """This type is deprecated and will be removed in a future release.
 
@@ -142,17 +143,17 @@
 """
 
 
 class Counterparty(BaseModel):
     accounts: List[Account]
     """The accounts for this counterparty."""
 
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     email: Optional[str]
     """The counterparty's email."""
 
     id: str
 
     live_mode: bool
@@ -174,8 +175,8 @@
 
     send_remittance_advice: bool
     """
     Send an email to the counterparty whenever an associated payment order is sent
     to the bank.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/counterparty_collect_account_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/counterparty_collect_account_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/counterparty_collect_account_response.py` & `modern_treasury-1.9.0/src/modern_treasury/types/counterparty_collect_account_response.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/counterparty_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/counterparty_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/counterparty_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/counterparty_list_params.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
-from typing_extensions import TypedDict
+from typing import Dict, Union, Optional
+from datetime import datetime
+from typing_extensions import Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["CounterpartyListParams"]
 
 
 class CounterpartyListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
-    created_at_lower_bound: str
+    created_at_lower_bound: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """Used to return counterparties created after some datetime."""
 
-    created_at_upper_bound: str
+    created_at_upper_bound: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """Used to return counterparties created before some datetime."""
 
     email: str
     """Performs a partial string match of the email field.
 
     This is also case insensitive.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/counterparty_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/counterparty_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/document.py` & `modern_treasury-1.9.0/src/modern_treasury/types/document.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["Document", "DocumentDetails", "DocumentDetail", "File"]
 
 
 class DocumentDetail(BaseModel):
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     document_identifier: str
 
     document_identifier_type: str
 
     id: str
 
@@ -23,15 +24,15 @@
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
 
 
 DocumentDetails = DocumentDetail
 """This type is deprecated and will be removed in a future release.
 
 Please use DocumentDetail instead.
 """
@@ -45,17 +46,17 @@
     """The original filename of the document."""
 
     size: Optional[int]
     """The size of the document in bytes."""
 
 
 class Document(BaseModel):
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     document_details: List[DocumentDetail]
 
     document_type: Optional[str]
     """A category given to the document, can be `null`."""
 
     documentable_id: str
@@ -87,8 +88,8 @@
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/event.py` & `modern_treasury-1.9.0/src/modern_treasury/types/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # File generated from our OpenAPI spec by Stainless.
 
+from datetime import datetime
+
 from .._models import BaseModel
 
 __all__ = ["Event"]
 
 
 class Event(BaseModel):
-    created_at: str
+    created_at: datetime
 
     data: object
     """The body of the event."""
 
     entity_id: str
     """The ID of the entity for the event."""
 
     event_name: str
     """The name of the event."""
 
-    event_time: str
+    event_time: datetime
     """The time of the event."""
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
@@ -29,8 +31,8 @@
     """
 
     object: str
 
     resource: str
     """The type of resource for the event."""
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/expected_payment.py` & `modern_treasury-1.9.0/src/modern_treasury/types/expected_payment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import shared, expected_payment_type
 from .._models import BaseModel
 
 __all__ = ["ExpectedPayment"]
 
@@ -23,23 +24,23 @@
     Value in specified currency's smallest unit. e.g. $10 would be represented
     as 1000.
     """
 
     counterparty_id: Optional[str]
     """The ID of the counterparty you expect for this payment."""
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """Must conform to ISO 4217. Defaults to the currency of the internal account."""
 
-    date_lower_bound: Optional[str]
+    date_lower_bound: Optional[date]
     """The earliest date the payment may come in. Format: yyyy-mm-dd"""
 
-    date_upper_bound: Optional[str]
+    date_upper_bound: Optional[date]
     """The latest date the payment may come in. Format: yyyy-mm-dd"""
 
     description: Optional[str]
     """An optional description for internal use."""
 
     direction: Literal["credit", "debit"]
     """One of credit or debit.
@@ -102,8 +103,8 @@
 
     type: Optional[expected_payment_type.ExpectedPaymentType]
     """
     One of: ach, au_becs, bacs, book, check, eft, interac, provxchange, rtp, sen,
     sepa, signet, wire.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_create_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import date
+from typing_extensions import Literal, Required, Annotated, TypedDict
 
 from ..types import shared_params
+from .._utils import PropertyInfo
 
 __all__ = ["ExpectedPaymentCreateParams", "LineItems", "LineItem"]
 
 
 class LineItem(TypedDict, total=False):
     amount: Required[int]
     """Value in specified currency's smallest unit.
@@ -67,18 +69,18 @@
 
     counterparty_id: Optional[str]
     """The ID of the counterparty you expect for this payment."""
 
     currency: shared_params.Currency
     """Must conform to ISO 4217. Defaults to the currency of the internal account."""
 
-    date_lower_bound: Optional[str]
+    date_lower_bound: Annotated[Optional[Union[str, date]], PropertyInfo(format="iso8601")]
     """The earliest date the payment may come in. Format: yyyy-mm-dd"""
 
-    date_upper_bound: Optional[str]
+    date_upper_bound: Annotated[Optional[Union[str, date]], PropertyInfo(format="iso8601")]
     """The latest date the payment may come in. Format: yyyy-mm-dd"""
 
     description: Optional[str]
     """An optional description for internal use."""
 
     line_items: List[LineItem]
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_list_params.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
-from typing_extensions import Literal, TypedDict
+from typing import Dict, Union, Optional
+from datetime import datetime
+from typing_extensions import Literal, Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["ExpectedPaymentListParams"]
 
 
 class ExpectedPaymentListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
     counterparty_id: str
     """Specify counterparty_id to see expected_payments for a specific account."""
 
-    created_at_lower_bound: str
+    created_at_lower_bound: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """Used to return expected payments created after some datetime"""
 
-    created_at_upper_bound: str
+    created_at_upper_bound: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
     """Used to return expected payments created before some datetime"""
 
     direction: Literal["credit", "debit"]
     """One of credit, debit"""
 
     internal_account_id: str
     """Specify internal_account_id to see expected_payments for a specific account."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/expected_payment_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/expected_payment_update_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
-from typing_extensions import Literal, TypedDict
+from typing import Dict, Union, Optional
+from datetime import date
+from typing_extensions import Literal, Annotated, TypedDict
 
 from ..types import shared_params
+from .._utils import PropertyInfo
 
 __all__ = ["ExpectedPaymentUpdateParams"]
 
 
 class ExpectedPaymentUpdateParams(TypedDict, total=False):
     amount_lower_bound: int
     """The lowest amount this expected payment may be equal to.
@@ -27,18 +29,18 @@
 
     counterparty_id: Optional[str]
     """The ID of the counterparty you expect for this payment."""
 
     currency: shared_params.Currency
     """Must conform to ISO 4217. Defaults to the currency of the internal account."""
 
-    date_lower_bound: Optional[str]
+    date_lower_bound: Annotated[Optional[Union[str, date]], PropertyInfo(format="iso8601")]
     """The earliest date the payment may come in. Format: yyyy-mm-dd"""
 
-    date_upper_bound: Optional[str]
+    date_upper_bound: Annotated[Optional[Union[str, date]], PropertyInfo(format="iso8601")]
     """The latest date the payment may come in. Format: yyyy-mm-dd"""
 
     description: Optional[str]
     """An optional description for internal use."""
 
     direction: Literal["credit", "debit"]
     """One of credit or debit.
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/external_account.py` & `modern_treasury-1.9.0/src/modern_treasury/types/external_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from ..types import account_detail, routing_detail, external_account_type
 from .._models import BaseModel
 
 __all__ = ["ExternalAccount", "PartyAddress", "ContactDetails", "ContactDetail"]
 
 
 class PartyAddress(BaseModel):
     country: Optional[str]
     """Country code conforms to [ISO 3166-1 alpha-2]"""
 
-    created_at: str
+    created_at: datetime
 
     id: str
 
     line1: Optional[str]
 
     line2: Optional[str]
 
@@ -34,37 +35,37 @@
 
     postal_code: Optional[str]
     """The postal code of the address."""
 
     region: Optional[str]
     """Region or State."""
 
-    updated_at: str
+    updated_at: datetime
 
 
 class ContactDetail(BaseModel):
     contact_identifier: str
 
     contact_identifier_type: Literal["email", "phone_number", "website"]
 
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
 
 
 ContactDetails = ContactDetail
 """This type is deprecated and will be removed in a future release.
 
 Please use ContactDetail instead.
 """
@@ -76,17 +77,17 @@
     account_type: external_account_type.ExternalAccountType
     """Can be `checking`, `savings` or `other`."""
 
     contact_details: List[ContactDetail]
 
     counterparty_id: Optional[str]
 
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -113,10 +114,10 @@
     """The legal name of the entity which owns the account."""
 
     party_type: Optional[Literal["business", "individual"]]
     """Either `individual` or `business`."""
 
     routing_details: List[routing_detail.RoutingDetail]
 
-    updated_at: str
+    updated_at: datetime
 
     verification_status: Literal["pending_verification", "unverified", "verified"]
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/external_account_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/external_account_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/external_account_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/external_account_list_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/external_account_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/external_account_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/external_account_verify_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/external_account_verify_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail.py` & `modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import shared, virtual_account
 from .._models import BaseModel
 
 __all__ = ["IncomingPaymentDetail"]
 
@@ -12,18 +13,18 @@
 class IncomingPaymentDetail(BaseModel):
     amount: int
     """Value in specified currency's smallest unit.
 
     e.g. $10 would be represented as 1000.
     """
 
-    as_of_date: str
+    as_of_date: date
     """The date on which the corresponding transaction will occur."""
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """The currency of the incoming payment detail."""
 
     data: object
     """The raw data from the payment pre-notification file that we get from the bank."""
 
@@ -66,15 +67,15 @@
 
     type: Literal["ach", "book", "check", "eft", "interac", "rtp", "sepa", "signet", "wire"]
     """
     One of: `ach`, `book`, `check`, `eft`, `interac`, `rtp`, `sepa`, `signet`, or
     `wire`.
     """
 
-    updated_at: str
+    updated_at: datetime
 
     vendor_id: Optional[str]
     """The identifier of the vendor bank."""
 
     virtual_account: Optional[virtual_account.VirtualAccount]
     """
     If the incoming payment detail is in a virtual account, the serialized virtual
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail_create_async_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail_create_async_params.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
-from typing_extensions import Literal, TypedDict
+from typing import Union, Optional
+from datetime import date
+from typing_extensions import Literal, Annotated, TypedDict
 
 from ..types import shared_params
+from .._utils import PropertyInfo
 
 __all__ = ["IncomingPaymentDetailCreateAsyncParams"]
 
 
 class IncomingPaymentDetailCreateAsyncParams(TypedDict, total=False):
     amount: int
     """Value in specified currency's smallest unit.
 
     e.g. $10 would be represented as 1000.
     """
 
-    as_of_date: Optional[str]
+    as_of_date: Annotated[Optional[Union[str, date]], PropertyInfo(format="iso8601")]
     """Defaults to today."""
 
     currency: shared_params.Currency
     """Defaults to the currency of the originating account."""
 
     direction: Literal["credit", "debit"]
     """One of `credit`, `debit`."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/incoming_payment_detail_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/incoming_payment_detail_list_params.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
-from typing_extensions import Literal, TypedDict
+from typing import Dict, Union, Optional
+from datetime import date
+from typing_extensions import Literal, Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["IncomingPaymentDetailListParams"]
 
 
 class IncomingPaymentDetailListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
-    as_of_date_end: str
+    as_of_date_end: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """
     Filters incoming payment details with an as_of_date starting on or before the
     specified date (YYYY-MM-DD).
     """
 
-    as_of_date_start: str
+    as_of_date_start: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """
     Filters incoming payment details with an as_of_date starting on or after the
     specified date (YYYY-MM-DD).
     """
 
     direction: Literal["credit", "debit"]
     """One of `credit` or `debit`."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/internal_account.py` & `modern_treasury-1.9.0/src/modern_treasury/types/internal_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from ..types import shared, connection, account_detail, routing_detail
 from .._models import BaseModel
 
 __all__ = ["InternalAccount", "PartyAddress"]
 
 
 class PartyAddress(BaseModel):
     country: Optional[str]
     """Country code conforms to [ISO 3166-1 alpha-2]"""
 
-    created_at: str
+    created_at: datetime
 
     id: str
 
     line1: Optional[str]
 
     line2: Optional[str]
 
@@ -34,15 +35,15 @@
 
     postal_code: Optional[str]
     """The postal code of the address."""
 
     region: Optional[str]
     """Region or State."""
 
-    updated_at: str
+    updated_at: datetime
 
 
 class InternalAccount(BaseModel):
     account_details: List[account_detail.AccountDetail]
     """An array of account detail objects."""
 
     account_type: Optional[Literal["cash", "checking", "loan", "non_resident", "other", "overdraft", "savings"]]
@@ -50,15 +51,15 @@
 
     connection: connection.Connection
     """Specifies which financial institution the accounts belong to."""
 
     counterparty_id: Optional[str]
     """The Counterparty associated to this account."""
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """The currency of the account."""
 
     id: str
 
     live_mode: bool
@@ -89,8 +90,8 @@
 
     party_type: Optional[Literal["business", "individual"]]
     """Either individual or business."""
 
     routing_details: List[routing_detail.RoutingDetail]
     """An array of routing detail objects."""
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/internal_account_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/internal_account_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/internal_account_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/internal_account_list_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/internal_account_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/internal_account_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/internal_accounts/balance_report.py` & `modern_treasury-1.9.0/src/modern_treasury/types/internal_accounts/balance_report.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ...types import shared
 from ..._models import BaseModel
 
 __all__ = ["BalanceReport", "Balances", "Balance"]
 
@@ -26,30 +27,30 @@
     """The specific type of balance reported.
 
     One of `opening_ledger`, `closing_ledger`, `current_ledger`,
     `opening_available`, `opening_available_next_business_day`, `closing_available`,
     `current_available`, or `other`.
     """
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """The currency of the balance."""
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
 
     vendor_code: str
     """The code used by the bank when reporting this specific balance."""
 
     vendor_code_type: Optional[
         Literal[
             "bai2",
@@ -78,38 +79,38 @@
 """This type is deprecated and will be removed in a future release.
 
 Please use Balance instead.
 """
 
 
 class BalanceReport(BaseModel):
-    as_of_date: str
+    as_of_date: date
     """The date of the balance report in local time."""
 
     as_of_time: Optional[str]
     """The time (24-hour clock) of the balance report in local time."""
 
     balance_report_type: Literal["intraday", "other", "previous_day", "real_time"]
     """The specific type of balance report.
 
     One of `intraday`, `previous_day`, `real_time`, or `other`.
     """
 
     balances: List[Balance]
     """An array of `Balance` objects."""
 
-    created_at: str
+    created_at: datetime
 
     id: str
 
     internal_account_id: str
     """The ID of one of your organization's Internal Accounts."""
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/internal_accounts/balance_report_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/internal_accounts/balance_report_list_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
-from typing_extensions import Literal, TypedDict
+from typing import Union, Optional
+from datetime import date
+from typing_extensions import Literal, Annotated, TypedDict
+
+from ..._utils import PropertyInfo
 
 __all__ = ["BalanceReportListParams"]
 
 
 class BalanceReportListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
-    as_of_date: str
+    as_of_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """The date of the balance report in local time."""
 
     balance_report_type: Literal["intraday", "other", "previous_day", "real_time"]
     """The specific type of balance report.
 
     One of `intraday`, `previous_day`, `real_time`, or `other`.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import datetime
 
 from .._models import BaseModel
 
 __all__ = ["Ledger"]
 
 
 class Ledger(BaseModel):
-    created_at: str
+    created_at: datetime
 
     description: Optional[str]
     """An optional free-form description for internal use."""
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -30,8 +31,8 @@
     """
 
     name: str
     """The name of the ledger."""
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["LedgerAccount", "Balances", "BalancesPendingBalance", "BalancesPostedBalance", "BalancesAvailableBalance"]
 
 
@@ -72,20 +73,20 @@
 
     The posted balance is the sum of all posted entries on the account. The pending
     balance is the sum of all pending and posted entries on the account. The
     available balance is the posted incoming entries minus the sum of the pending
     and posted outgoing amounts.
     """
 
-    created_at: str
+    created_at: datetime
 
     description: Optional[str]
     """The description of the ledger account."""
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     ledger_id: str
     """The id of the ledger that this account belongs to."""
 
     live_mode: bool
@@ -107,8 +108,8 @@
     """The name of the ledger account."""
 
     normal_balance: Literal["credit", "debit"]
     """The normal balance of the ledger account."""
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = [
     "LedgerAccountCategory",
     "Balances",
@@ -78,20 +79,20 @@
 
     The posted balance is the sum of all posted entries on the account. The pending
     balance is the sum of all pending and posted entries on the account. The
     available balance is the posted incoming entries minus the sum of the pending
     and posted outgoing amounts.
     """
 
-    created_at: str
+    created_at: datetime
 
     description: Optional[str]
     """The description of the ledger account category."""
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     ledger_id: str
     """The id of the ledger that this account category belongs to."""
 
     live_mode: bool
@@ -110,8 +111,8 @@
     """The name of the ledger account category."""
 
     normal_balance: Literal["credit", "debit"]
     """The normal balance of the ledger account category."""
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_list_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_retrieve_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_retrieve_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing_extensions import TypedDict
+from typing import Union
+from datetime import date
+from typing_extensions import Annotated, TypedDict
 
-__all__ = ["LedgerAccountCategoryRetrieveParams", "Balances"]
+from .._utils import PropertyInfo
 
+__all__ = ["LedgerAccountRetrieveParams", "Balances"]
 
-class Balances(TypedDict, total=False):
-    as_of_date: str
 
-    effective_at: str
+class Balances(TypedDict, total=False):
+    as_of_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
 
 
-class LedgerAccountCategoryRetrieveParams(TypedDict, total=False):
+class LedgerAccountRetrieveParams(TypedDict, total=False):
     balances: Balances
     """
     For example, if you want the balances as of a particular effective date
     (YYYY-MM-DD), the encoded query string would be
     balances%5Bas_of_date%5D=2000-12-31. The balances as of a date are inclusive of
     entries with that exact date.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_category_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_category_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_list_params.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
-from typing_extensions import TypedDict
+from typing import Dict, Union, Optional
+from datetime import date, datetime
+from typing_extensions import Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["LedgerAccountListParams", "Balances"]
 
 
 class Balances(TypedDict, total=False):
-    as_of_date: str
+    as_of_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
 
-    effective_at: str
+    effective_at: Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]
 
 
 class LedgerAccountListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
     balances: Balances
     """
@@ -38,13 +41,13 @@
     parameters.
     """
 
     name: str
 
     per_page: int
 
-    updated_at: Dict[str, str]
+    updated_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     posted at timestamp. For example, for all times after Jan 1 2000 12:00 UTC, use
     updated_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["LedgerAccountPayout"]
 
 
 class LedgerAccountPayout(BaseModel):
     amount: Optional[int]
     """The amount of the ledger account payout."""
 
-    created_at: str
+    created_at: datetime
 
     currency: str
     """The currency of the ledger account payout."""
 
     currency_exponent: Optional[int]
     """The currency exponent of the ledger account payout."""
 
@@ -63,8 +64,8 @@
 
     status: Literal["archived", "archiving", "pending", "posted", "processing"]
     """The status of the ledger account payout.
 
     One of `processing`, `pending`, `posted`, `archiving` or `archived`.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_payout_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_payout_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_account_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_account_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_entry.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = [
     "LedgerEntry",
     "ResultingLedgerAccountBalances",
@@ -75,26 +76,26 @@
 class LedgerEntry(BaseModel):
     amount: int
     """Value in specified currency's smallest unit.
 
     e.g. $10 would be represented as 1000. Can be any integer up to 36 digits.
     """
 
-    created_at: str
+    created_at: datetime
 
     direction: Literal["credit", "debit"]
     """One of `credit`, `debit`.
 
     Describes the direction money is flowing in the transaction. A `credit` moves
     money from your account to someone else's. A `debit` pulls money from someone
     else's account to your own. Note that wire, rtp, and check payments will always
     be `credit`.
     """
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     ledger_account_currency: str
     """The currency of the ledger account."""
 
     ledger_account_currency_exponent: int
@@ -135,8 +136,8 @@
 
     status: Literal["archived", "pending", "posted"]
     """Equal to the state of the ledger transaction when the ledger entry was created.
 
     One of `pending`, `posted`, or `archived`.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_entry_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_entry_list_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import date, datetime
 from typing_extensions import Literal, TypedDict
 
 __all__ = ["LedgerEntryListParams"]
 
 
 class LedgerEntryListParams(TypedDict, total=False):
     after_cursor: Optional[str]
@@ -20,15 +21,15 @@
 
     effective_at: Dict[str, str]
     """
     Use "gt" (>), "gte" (>=), "lt" (<), "lte" (<=), or "eq" (=) to filter by the
     transaction's effective time. Format ISO8601
     """
 
-    effective_date: Dict[str, str]
+    effective_date: Dict[str, Union[str, date]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     transaction's effective date. Format YYYY-MM-DD
     """
 
     ledger_account_category_id: str
     """Get all ledger entries that match the direction specified.
@@ -59,13 +60,13 @@
 
     status: Literal["pending", "posted", "archived"]
     """Get all ledger entries that match the status specified.
 
     One of `pending`, `posted`, or `archived`.
     """
 
-    updated_at: Dict[str, str]
+    updated_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     posted at timestamp. For example, for all times after Jan 1 2000 12:00 UTC, use
     updated_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_list_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 from typing_extensions import TypedDict
 
 __all__ = ["LedgerListParams"]
 
 
 class LedgerListParams(TypedDict, total=False):
     after_cursor: Optional[str]
@@ -16,13 +17,13 @@
     For example, if you want to query for records with metadata key `Type` and value
     `Loan`, the query would be `metadata%5BType%5D=Loan`. This encodes the query
     parameters.
     """
 
     per_page: int
 
-    updated_at: Dict[str, str]
+    updated_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     posted at timestamp. For example, for all times after Jan 1 2000 12:00 UTC, use
     updated_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import ledger_entry
 from .._models import BaseModel
 
 __all__ = ["LedgerTransaction"]
 
 
 class LedgerTransaction(BaseModel):
-    created_at: str
+    created_at: datetime
 
     description: Optional[str]
     """An optional description for internal use."""
 
-    effective_at: str
+    effective_at: date
     """
     The timestamp (ISO8601 format) at which the ledger transaction happened for
     reporting purposes.
     """
 
-    effective_date: str
+    effective_date: date
     """
     The date (YYYY-MM-DD) on which the ledger transaction happened for reporting
     purposes.
     """
 
     external_id: Optional[str]
     """A unique string to represent the ledger transaction.
@@ -86,8 +87,8 @@
 
     This is null if the ledger transaction is pending.
     """
 
     status: Literal["archived", "pending", "posted"]
     """To post a ledger transaction at creation, use `posted`."""
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction_create_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import date
+from typing_extensions import Literal, Required, Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["LedgerTransactionCreateParams", "LedgerEntries", "LedgerEntry"]
 
 
 class LedgerEntry(TypedDict, total=False):
     amount: Required[int]
     """Value in specified currency's smallest unit.
@@ -67,15 +70,15 @@
 """This type is deprecated and will be removed in a future release.
 
 Please use LedgerEntry instead.
 """
 
 
 class LedgerTransactionCreateParams(TypedDict, total=False):
-    effective_date: Required[str]
+    effective_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """
     The date (YYYY-MM-DD) on which the ledger transaction happened for reporting
     purposes.
     """
 
     ledger_entries: Required[List[LedgerEntry]]
     """An array of ledger entry objects."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction_list_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 from typing_extensions import Literal, TypedDict
 
 __all__ = ["LedgerTransactionListParams"]
 
 
 class LedgerTransactionListParams(TypedDict, total=False):
     after_cursor: Optional[str]
@@ -14,15 +15,15 @@
     effective_at: Dict[str, str]
     """
     Use "gt" (>), "gte" (>=), "lt" (<), "lte" (<=), or "eq" (=) to filter by
     effective at. For example, for all transactions after Jan 1 2000, use
     effective_at%5Bgt%5D=2000-01-01T00:00:00:00.000Z.
     """
 
-    effective_date: Dict[str, str]
+    effective_date: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by
     effective date. For example, for all dates after Jan 1 2000, use
     effective_date%5Bgt%5D=2000-01-01.
     """
 
     external_id: str
@@ -38,22 +39,22 @@
     For example, if you want to query for records with metadata key `Type` and value
     `Loan`, the query would be `metadata%5BType%5D=Loan`. This encodes the query
     parameters.
     """
 
     per_page: int
 
-    posted_at: Dict[str, str]
+    posted_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     posted at timestamp. For example, for all times after Jan 1 2000 12:00 UTC, use
     posted_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
 
     status: Literal["pending", "posted", "archived"]
 
-    updated_at: Dict[str, str]
+    updated_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     posted at timestamp. For example, for all times after Jan 1 2000 12:00 UTC, use
     updated_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transaction_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transaction_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/ledger_transaction_version.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/ledger_transaction_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..._models import BaseModel
 
 __all__ = [
     "LedgerTransactionVersion",
     "LedgerEntries",
@@ -109,15 +110,15 @@
 class LedgerEntry(BaseModel):
     amount: int
     """Value in specified currency's smallest unit.
 
     e.g. $10 would be represented as 1000. Can be any integer up to 36 digits.
     """
 
-    created_at: str
+    created_at: datetime
 
     direction: Literal["credit", "debit"]
     """One of `credit`, `debit`.
 
     Describes the direction money is flowing in the transaction. A `credit` moves
     money from your account to someone else's. A `debit` pulls money from someone
     else's account to your own. Note that wire, rtp, and check payments will always
@@ -176,20 +177,20 @@
 """This type is deprecated and will be removed in a future release.
 
 Please use LedgerEntry instead.
 """
 
 
 class LedgerTransactionVersion(BaseModel):
-    created_at: str
+    created_at: datetime
 
     description: Optional[str]
     """An optional description for internal use."""
 
-    effective_date: str
+    effective_date: date
     """
     The date (YYYY-MM-DD) on which the ledger transaction happened for reporting
     purposes.
     """
 
     external_id: Optional[str]
     """A unique string to represent the ledger transaction.
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/version_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/version_versions_params.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 from typing_extensions import TypedDict
 
-__all__ = ["VersionListParams"]
+__all__ = ["VersionVersionsParams"]
 
 
-class VersionListParams(TypedDict, total=False):
+class VersionVersionsParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
-    created_at: Dict[str, str]
+    created_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     created_at timestamp. For example, for all dates after Jan 1 2000 12:00 UTC, use
     created_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
 
     per_page: int
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_transactions/version_versions_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_transactions/version_list_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, Optional
+from typing import Dict, Union, Optional
+from datetime import datetime
 from typing_extensions import TypedDict
 
-__all__ = ["VersionVersionsParams"]
+__all__ = ["VersionListParams"]
 
 
-class VersionVersionsParams(TypedDict, total=False):
+class VersionListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
-    created_at: Dict[str, str]
+    created_at: Dict[str, Union[str, datetime]]
     """
     Use `gt` (>), `gte` (>=), `lt` (<), `lte` (<=), or `eq` (=) to filter by the
     created_at timestamp. For example, for all dates after Jan 1 2000 12:00 UTC, use
     created_at%5Bgt%5D=2000-01-01T12:00:00Z.
     """
 
     per_page: int
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/ledger_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/ledger_update_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/line_item.py` & `modern_treasury-1.9.0/src/modern_treasury/types/line_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["LineItem", "Accounting"]
 
 
@@ -45,15 +46,15 @@
 
     amount: int
     """Value in specified currency's smallest unit.
 
     e.g. $10 would be represented as 1000.
     """
 
-    created_at: str
+    created_at: datetime
 
     description: Optional[str]
     """A free-form description of the line item."""
 
     id: str
 
     itemizable_id: str
@@ -72,8 +73,8 @@
     """Additional data represented as key-value pairs.
 
     Both the key and value must be strings.
     """
 
     object: str
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/paper_item.py` & `modern_treasury-1.9.0/src/modern_treasury/types/paper_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import shared
 from .._models import BaseModel
 
 __all__ = ["PaperItem"]
 
@@ -18,20 +19,20 @@
 
     amount: int
     """The amount of the paper item."""
 
     check_number: Optional[str]
     """The check number on the paper item."""
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """The currency of the paper item."""
 
-    deposit_date: str
+    deposit_date: date
     """The date the paper item was deposited into your organization's bank account."""
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
@@ -60,8 +61,8 @@
 
     transaction_id: Optional[str]
     """The ID of the reconciled Transaction or `null`."""
 
     transaction_line_item_id: Optional[str]
     """The ID of the reconciled Transaction Line Item or `null`."""
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/paper_item_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/paper_item_list_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
-from typing_extensions import TypedDict
+from typing import Union, Optional
+from datetime import date
+from typing_extensions import Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["PaperItemListParams"]
 
 
 class PaperItemListParams(TypedDict, total=False):
     after_cursor: Optional[str]
 
-    deposit_date_end: str
+    deposit_date_end: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """Specify an inclusive end date (YYYY-MM-DD) when filtering by deposit_date"""
 
-    deposit_date_start: str
+    deposit_date_start: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """Specify an inclusive start date (YYYY-MM-DD) when filtering by deposit_date"""
 
     lockbox_number: str
     """
     Specify `lockbox_number` if you wish to see paper items that are associated with
     a specific lockbox number.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_order.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_order.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import shared, return_object, payment_order_type, payment_order_subtype
 from .._models import BaseModel
 
 __all__ = ["PaymentOrder", "Accounting", "ReferenceNumbers", "ReferenceNumber"]
 
@@ -23,15 +24,15 @@
     Class objects track segments of your business independent of client or project.
     Note that these will only be accessible if your accounting system has been
     connected.
     """
 
 
 class ReferenceNumber(BaseModel):
-    created_at: str
+    created_at: datetime
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -91,15 +92,15 @@
         "swift_uetr",
         "usbank_payment_id",
         "wells_fargo_payment_id",
         "wells_fargo_trace_number",
     ]
     """The type of the reference number. Referring to the vendor payment id."""
 
-    updated_at: str
+    updated_at: datetime
 
 
 ReferenceNumbers = ReferenceNumber
 """This type is deprecated and will be removed in a future release.
 
 Please use ReferenceNumber instead.
 """
@@ -144,15 +145,15 @@
 
     counterparty_id: Optional[str]
     """
     If the payment order is tied to a specific Counterparty, their id will appear,
     otherwise `null`.
     """
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """Defaults to the currency of the originating account."""
 
     current_return: Optional[return_object.ReturnObject]
     """
     If the payment order's status is `returned`, this will include the return
@@ -173,22 +174,22 @@
 
     Describes the direction money is flowing in the transaction. A `credit` moves
     money from your account to someone else's. A `debit` pulls money from someone
     else's account to your own. Note that wire, rtp, and check payments will always
     be `credit`.
     """
 
-    effective_date: str
+    effective_date: date
     """Date transactions are to be posted to the participants' account.
 
     Defaults to the current business day or the next business day if the current day
     is a bank holiday or weekend. Format: yyyy-mm-dd.
     """
 
-    expires_at: Optional[str]
+    expires_at: Optional[datetime]
     """RFP payments require an expires_at. This value must be past the effective_date."""
 
     foreign_exchange_contract: Optional[str]
     """
     If present, indicates a specific foreign exchange contract number that has been
     generated by your financial institution.
     """
@@ -332,15 +333,15 @@
     ultimate_originating_party_name: Optional[str]
     """Name of the ultimate originator of the payment order."""
 
     ultimate_receiving_party_identifier: Optional[str]
 
     ultimate_receiving_party_name: Optional[str]
 
-    updated_at: str
+    updated_at: datetime
 
     vendor_failure_reason: Optional[str]
     """This field will be populated if a vendor (e.g.
 
     Currencycloud) failure occurs. Logic shouldn't be built on its value as it is
     free-form.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_order_create_async_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_order_create_async_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import date, datetime
+from typing_extensions import Literal, Required, Annotated, TypedDict
 
 from ..types import shared_params
+from .._utils import PropertyInfo
 
 __all__ = [
     "PaymentOrderCreateAsyncParams",
     "Accounting",
     "ReceivingAccount",
     "ReceivingAccountPartyAddress",
     "ReceivingAccountAccountDetails",
@@ -223,15 +225,15 @@
 """This type is deprecated and will be removed in a future release.
 
 Please use LedgerTransactionLedgerEntry instead.
 """
 
 
 class LedgerTransaction(TypedDict, total=False):
-    effective_date: Required[str]
+    effective_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """
     The date (YYYY-MM-DD) on which the ledger transaction happened for reporting
     purposes.
     """
 
     ledger_entries: Required[List[LedgerTransactionLedgerEntry]]
     """An array of ledger entry objects."""
@@ -381,22 +383,22 @@
 
     currency: shared_params.Currency
     """Defaults to the currency of the originating account."""
 
     description: Optional[str]
     """An optional description for internal use."""
 
-    effective_date: str
+    effective_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """Date transactions are to be posted to the participants' account.
 
     Defaults to the current business day or the next business day if the current day
     is a bank holiday or weekend. Format: yyyy-mm-dd.
     """
 
-    expires_at: Optional[str]
+    expires_at: Annotated[Optional[Union[str, datetime]], PropertyInfo(format="iso8601")]
     """RFP payments require an expires_at. This value must be past the effective_date."""
 
     fallback_type: Literal["ach"]
     """
     A payment type to fallback to if the original type is not valid for the
     receiving account. Currently, this only supports falling back from RTP to ACH
     (type=rtp and fallback_type=ach)
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_order_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_order_create_params.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import date, datetime
+from typing_extensions import Literal, Required, Annotated, TypedDict
 
 from ..types import shared_params
 from .._types import FileTypes
+from .._utils import PropertyInfo
 
 __all__ = [
     "PaymentOrderCreateParams",
     "Accounting",
     "ReceivingAccount",
     "ReceivingAccountPartyAddress",
     "ReceivingAccountAccountDetails",
@@ -226,15 +228,15 @@
 """This type is deprecated and will be removed in a future release.
 
 Please use LedgerTransactionLedgerEntry instead.
 """
 
 
 class LedgerTransaction(TypedDict, total=False):
-    effective_date: Required[str]
+    effective_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """
     The date (YYYY-MM-DD) on which the ledger transaction happened for reporting
     purposes.
     """
 
     ledger_entries: Required[List[LedgerTransactionLedgerEntry]]
     """An array of ledger entry objects."""
@@ -405,22 +407,22 @@
     documents: List[Document]
     """An array of documents to be attached to the payment order.
 
     Note that if you attach documents, the request's content type must be
     `multipart/form-data`.
     """
 
-    effective_date: str
+    effective_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """Date transactions are to be posted to the participants' account.
 
     Defaults to the current business day or the next business day if the current day
     is a bank holiday or weekend. Format: yyyy-mm-dd.
     """
 
-    expires_at: Optional[str]
+    expires_at: Annotated[Optional[Union[str, datetime]], PropertyInfo(format="iso8601")]
     """RFP payments require an expires_at. This value must be past the effective_date."""
 
     fallback_type: Literal["ach"]
     """
     A payment type to fallback to if the original type is not valid for the
     receiving account. Currently, this only supports falling back from RTP to ACH
     (type=rtp and fallback_type=ach)
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_order_update_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_order_update_params.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import date, datetime
+from typing_extensions import Literal, Required, Annotated, TypedDict
 
 from ..types import shared_params
+from .._utils import PropertyInfo
 
 __all__ = [
     "PaymentOrderUpdateParams",
     "Accounting",
     "ReceivingAccount",
     "ReceivingAccountPartyAddress",
     "ReceivingAccountAccountDetails",
@@ -237,22 +239,22 @@
 
     Describes the direction money is flowing in the transaction. A `credit` moves
     money from your account to someone else's. A `debit` pulls money from someone
     else's account to your own. Note that wire, rtp, and check payments will always
     be `credit`.
     """
 
-    effective_date: str
+    effective_date: Annotated[Union[str, date], PropertyInfo(format="iso8601")]
     """Date transactions are to be posted to the participants' account.
 
     Defaults to the current business day or the next business day if the current day
     is a bank holiday or weekend. Format: yyyy-mm-dd.
     """
 
-    expires_at: Optional[str]
+    expires_at: Annotated[Optional[Union[str, datetime]], PropertyInfo(format="iso8601")]
     """RFP payments require an expires_at. This value must be past the effective_date."""
 
     fallback_type: Literal["ach"]
     """
     A payment type to fallback to if the original type is not valid for the
     receiving account. Currently, this only supports falling back from RTP to ACH
     (type=rtp and fallback_type=ach)
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_orders/reversal_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_orders/reversal_create_params.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import date
+from typing_extensions import Literal, Required, Annotated, TypedDict
+
+from ..._utils import PropertyInfo
 
 __all__ = [
     "ReversalCreateParams",
     "LedgerTransaction",
     "LedgerTransactionLedgerEntries",
     "LedgerTransactionLedgerEntry",
 ]
@@ -72,15 +75,15 @@
 """This type is deprecated and will be removed in a future release.
 
 Please use LedgerTransactionLedgerEntry instead.
 """
 
 
 class LedgerTransaction(TypedDict, total=False):
-    effective_date: Required[str]
+    effective_date: Required[Annotated[Union[str, date], PropertyInfo(format="iso8601")]]
     """
     The date (YYYY-MM-DD) on which the ledger transaction happened for reporting
     purposes.
     """
 
     ledger_entries: Required[List[LedgerTransactionLedgerEntry]]
     """An array of ledger entry objects."""
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_reference.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # File generated from our OpenAPI spec by Stainless.
 
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["PaymentReference"]
 
 
 class PaymentReference(BaseModel):
-    created_at: str
+    created_at: datetime
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -84,8 +85,8 @@
 
     referenceable_type: Literal["payment_order", "reversal", "return"]
     """One of the referenceable types.
 
     This must be accompanied by the id of the referenceable or will return an error.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/payment_reference_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/payment_reference_list_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/return_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/return_create_params.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Union, Optional
+from datetime import date
+from typing_extensions import Literal, Required, Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["ReturnCreateParams"]
 
 
 class ReturnCreateParams(TypedDict, total=False):
     returnable_id: Required[Optional[str]]
     """The ID of the object being returned or `null`."""
@@ -69,15 +72,15 @@
             "R52",
             "R53",
             "currencycloud",
         ]
     ]
     """The return code. For ACH returns, this is the required ACH return code."""
 
-    date_of_death: Optional[str]
+    date_of_death: Annotated[Optional[Union[str, date]], PropertyInfo(format="iso8601")]
     """
     If the return code is `R14` or `R15` this is the date the deceased counterparty
     passed away.
     """
 
     reason: Optional[str]
     """An optional description of the reason for the return.
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/return_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/return_list_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/return_object.py` & `modern_treasury-1.9.0/src/modern_treasury/types/return_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import List, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import shared
 from .._models import BaseModel
 
 __all__ = ["ReturnObject", "ReferenceNumbers", "ReferenceNumber"]
 
 
 class ReferenceNumber(BaseModel):
-    created_at: str
+    created_at: datetime
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -74,15 +75,15 @@
         "swift_uetr",
         "usbank_payment_id",
         "wells_fargo_payment_id",
         "wells_fargo_trace_number",
     ]
     """The type of the reference number. Referring to the vendor payment id."""
 
-    updated_at: str
+    updated_at: datetime
 
 
 ReferenceNumbers = ReferenceNumber
 """This type is deprecated and will be removed in a future release.
 
 Please use ReferenceNumber instead.
 """
@@ -146,20 +147,20 @@
             "R52",
             "R53",
             "currencycloud",
         ]
     ]
     """The return code. For ACH returns, this is the required ACH return code."""
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """Currency that this transaction is denominated in."""
 
-    date_of_death: Optional[str]
+    date_of_death: Optional[date]
     """
     If the return code is `R14` or `R15` this is the date the deceased counterparty
     passed away.
     """
 
     failure_reason: Optional[str]
     """
@@ -213,8 +214,8 @@
     type: Literal["ach", "ach_noc", "au_becs", "bacs", "book", "eft", "interac", "paper_item", "sepa", "wire"]
     """The type of return.
 
     Can be one of: `ach`, `ach_noc`, `au_becs`, `bacs`, `eft`, `interac`, `manual`,
     `paper_item`, `wire`.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/routing_detail.py` & `modern_treasury-1.9.0/src/modern_treasury/types/routing_detail.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Optional
+from datetime import datetime
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = ["RoutingDetail", "BankAddress"]
 
 
 class BankAddress(BaseModel):
     country: Optional[str]
     """Country code conforms to [ISO 3166-1 alpha-2]"""
 
-    created_at: str
+    created_at: datetime
 
     id: str
 
     line1: Optional[str]
 
     line2: Optional[str]
 
@@ -33,26 +34,26 @@
 
     postal_code: Optional[str]
     """The postal code of the address."""
 
     region: Optional[str]
     """Region or State."""
 
-    updated_at: str
+    updated_at: datetime
 
 
 class RoutingDetail(BaseModel):
     bank_address: Optional[BankAddress]
 
     bank_name: str
     """The name of the bank."""
 
-    created_at: str
+    created_at: datetime
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     live_mode: bool
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -90,8 +91,8 @@
     """The routing number of the bank."""
 
     routing_number_type: Literal[
         "aba", "au_bsb", "br_codigo", "ca_cpa", "cnaps", "gb_sort_code", "in_ifsc", "my_branch_code", "swift"
     ]
     """One of `aba`, `swift`, `ca_cpa`, `au_bsb`, `gb_sort_code`, `in_ifsc`, `cnaps`."""
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/routing_detail_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/routing_detail_create_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/routing_number_lookup_request.py` & `modern_treasury-1.9.0/src/modern_treasury/types/routing_number_lookup_request.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/shared/currency.py` & `modern_treasury-1.9.0/src/modern_treasury/types/shared/currency.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/shared_params/currency.py` & `modern_treasury-1.9.0/src/modern_treasury/types/shared_params/currency.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/transaction.py` & `modern_treasury-1.9.0/src/modern_treasury/types/transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, Optional
+from datetime import date, datetime
 from typing_extensions import Literal
 
 from ..types import shared
 from .._models import BaseModel
 
 __all__ = ["Transaction"]
 
@@ -12,25 +13,25 @@
 class Transaction(BaseModel):
     amount: int
     """Value in specified currency's smallest unit.
 
     e.g. $10 would be represented as 1000.
     """
 
-    as_of_date: Optional[str]
+    as_of_date: Optional[date]
     """The date on which the transaction occurred."""
 
     as_of_time: Optional[str]
     """The time on which the transaction occurred.
 
     Depending on the granularity of the timestamp information received from the
     bank, it may be `null`.
     """
 
-    created_at: str
+    created_at: datetime
 
     currency: Optional[shared.Currency]
     """Currency that this transaction is denominated in."""
 
     details: Dict[str, str]
     """
     This field contains additional information that the bank provided about the
@@ -41,15 +42,15 @@
     partner. Currently, the following keys may be in the details object:
     `originator_name`, `originator_to_beneficiary_information`.
     """
 
     direction: str
     """Either `credit` or `debit`."""
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     internal_account_id: str
     """The ID of the relevant Internal Account."""
 
     live_mode: bool
@@ -96,15 +97,15 @@
         "wire",
     ]
     """The type of the transaction.
 
     Can be one of `ach`, `wire`, `check`, `rtp`, `book`, or `sen`.
     """
 
-    updated_at: str
+    updated_at: datetime
 
     vendor_code: Optional[str]
     """When applicable, the bank-given code that determines the transaction's category.
 
     For most banks this is the BAI2/BTRS transaction code.
     """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/validation_validate_routing_number_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/validation_validate_routing_number_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/virtual_account.py` & `modern_treasury-1.9.0/src/modern_treasury/types/virtual_account.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from typing import Dict, List, Optional
+from datetime import datetime
 
 from ..types import account_detail, routing_detail
 from .._models import BaseModel
 
 __all__ = ["VirtualAccount"]
 
 
 class VirtualAccount(BaseModel):
     account_details: List[account_detail.AccountDetail]
     """An array of account detail objects."""
 
     counterparty_id: Optional[str]
     """The ID of a counterparty that the virtual account belongs to. Optional."""
 
-    created_at: str
+    created_at: datetime
 
     credit_ledger_account_id: Optional[str]
     """The ID of a credit normal ledger account.
 
     When money enters the virtual account, this ledger account will be credited.
     Must be accompanied by a debit_ledger_account_id if present.
     """
@@ -30,15 +31,15 @@
     When money enters the virtual account, this ledger account will be debited. Must
     be accompanied by a credit_ledger_account_id if present.
     """
 
     description: Optional[str]
     """An optional free-form description for internal use."""
 
-    discarded_at: Optional[str]
+    discarded_at: Optional[datetime]
 
     id: str
 
     internal_account_id: str
     """The ID of the internal account that the virtual account is in."""
 
     live_mode: bool
@@ -60,8 +61,8 @@
 
     routing_details: List[routing_detail.RoutingDetail]
     """An array of routing detail objects.
 
     These will be the routing details of the internal account.
     """
 
-    updated_at: str
+    updated_at: datetime
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/virtual_account_create_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/virtual_account_create_params.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 # File generated from our OpenAPI spec by Stainless.
 
 from __future__ import annotations
 
-from typing import Dict, List, Optional
-from typing_extensions import Literal, Required, TypedDict
+from typing import Dict, List, Union, Optional
+from datetime import datetime
+from typing_extensions import Literal, Required, Annotated, TypedDict
+
+from .._utils import PropertyInfo
 
 __all__ = ["VirtualAccountCreateParams", "AccountDetail", "RoutingDetail", "RoutingDetailBankAddress"]
 
 
 class AccountDetail(TypedDict, total=False):
     account_number_safe: Required[str]
     """The last 4 digits of the account_number."""
 
     account_number_type: Required[Literal["clabe", "iban", "other", "pan", "wallet_address"]]
     """One of `iban`, `clabe`, `wallet_address`, or `other`.
 
     Use `other` if the bank account number is in a generic format.
     """
 
-    created_at: Required[str]
+    created_at: Required[Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]]
 
-    discarded_at: Required[Optional[str]]
+    discarded_at: Required[Annotated[Optional[Union[str, datetime]], PropertyInfo(format="iso8601")]]
 
     id: Required[str]
 
     live_mode: Required[bool]
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
     """
 
     object: Required[str]
 
-    updated_at: Required[str]
+    updated_at: Required[Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]]
 
     account_number: str
     """The account number for the bank account."""
 
 
 AccountDetail = AccountDetail
 """This type is deprecated and will be removed in a future release.
@@ -45,15 +48,15 @@
 """
 
 
 class RoutingDetailBankAddress(TypedDict, total=False):
     country: Required[Optional[str]]
     """Country code conforms to [ISO 3166-1 alpha-2]"""
 
-    created_at: Required[str]
+    created_at: Required[Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]]
 
     id: Required[str]
 
     line1: Required[Optional[str]]
 
     line2: Required[Optional[str]]
 
@@ -70,15 +73,15 @@
 
     postal_code: Required[Optional[str]]
     """The postal code of the address."""
 
     region: Required[Optional[str]]
     """Region or State."""
 
-    updated_at: Required[str]
+    updated_at: Required[Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]]
 
 
 RoutingDetailBankAddress = RoutingDetailBankAddress
 """This type is deprecated and will be removed in a future release.
 
 Please use RoutingDetailBankAddress instead.
 """
@@ -86,17 +89,17 @@
 
 class RoutingDetail(TypedDict, total=False):
     bank_address: Required[Optional[RoutingDetailBankAddress]]
 
     bank_name: Required[str]
     """The name of the bank."""
 
-    created_at: Required[str]
+    created_at: Required[Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]]
 
-    discarded_at: Required[Optional[str]]
+    discarded_at: Required[Annotated[Optional[Union[str, datetime]], PropertyInfo(format="iso8601")]]
 
     id: Required[str]
 
     live_mode: Required[bool]
     """
     This field will be true if this object exists in the live environment or false
     if it exists in the test environment.
@@ -136,15 +139,15 @@
     """The routing number of the bank."""
 
     routing_number_type: Required[
         Literal["aba", "au_bsb", "br_codigo", "ca_cpa", "cnaps", "gb_sort_code", "in_ifsc", "my_branch_code", "swift"]
     ]
     """One of `aba`, `swift`, `ca_cpa`, `au_bsb`, `gb_sort_code`, `in_ifsc`, `cnaps`."""
 
-    updated_at: Required[str]
+    updated_at: Required[Annotated[Union[str, datetime], PropertyInfo(format="iso8601")]]
 
 
 RoutingDetail = RoutingDetail
 """This type is deprecated and will be removed in a future release.
 
 Please use RoutingDetail instead.
 """
```

### Comparing `modern_treasury-1.8.0/src/modern_treasury/types/virtual_account_list_params.py` & `modern_treasury-1.9.0/src/modern_treasury/types/virtual_account_list_params.py`

 * *Files identical despite different names*

### Comparing `modern_treasury-1.8.0/PKG-INFO` & `modern_treasury-1.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: modern-treasury
-Version: 1.8.0
-Summary: Client library for the Modern Treasury API
-Home-page: https://github.com/Modern-Treasury/modern-treasury-python
-License: MIT
-Author: Modern Treasury
-Author-email: sdk-feedback@moderntreasury.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anyio (>=3.5.0)
-Requires-Dist: distro (>=1.7.0)
-Requires-Dist: httpx (>=0.23.0)
-Requires-Dist: pydantic (>=1.9.0)
-Requires-Dist: typing-extensions (>=4.1.1)
-Project-URL: Repository, https://github.com/Modern-Treasury/modern-treasury-python
-Description-Content-Type: text/markdown
-
 # Modern Treasury Python API Library
 
 > **Migration Guide**
 >
 > We've made some major improvements to how you pass arguments to methods which will require migrating your existing code.
 >
 > If you want to migrate to the new patterns incrementally you can do so by installing `v0.5.0`. This release contains both
@@ -545,18 +521,52 @@
 - `ReceivingAccountContactDetails` -> `ReceivingAccountContactDetail`
 - `ReceivingAccountRoutingDetails` -> `ReceivingAccountRoutingDetail`
 - `LedgerEntriesResultingLedgerAccountBalances` -> `LedgerEntryResultingLedgerAccountBalances`
 - `LedgerEntriesResultingLedgerAccountBalancesPostedBalance` -> `LedgerEntryResultingLedgerAccountBalancesPostedBalance`
 - `LedgerEntriesResultingLedgerAccountBalancesPendingBalance` -> `LedgerEntryResultingLedgerAccountBalancesPendingBalance`
 - `LedgerEntriesResultingLedgerAccountBalancesAvailableBalance` -> `LedgerEntryResultingLedgerAccountBalancesAvailableBalance`
 
+## Rich `date` and `datetime` types
+
+We've improved the types for response fields / request params that correspond to `date` or `datetime` values!
+
+Previously they were just raw strings but now response fields will be instances of `date` or `datetime`.
+
+This means that if you're working with these fields and parsing them into `datetime` instances manually you will have to remove
+any code that performs said parsing.
+
+```diff
+account = client.internal_accounts.retrieve('<id>')
+- created_at = datetime.fromisoformat(account.created_at)
++ created_at = account.created_at
+print(created_at.month)
+```
+
+For request params you can continue to pass in strings if you want to use a datetime library other than the standard library version but if you
+were writing code that looked like this:
+
+```py
+dt = datetime(...)
+for counterparty in client.counterparties.list(created_at_upper_bound=dt.isoformat()):
+  ...
+```
+
+You can remove the explicit call to `isoformat`!
+
+```diff
+dt = datetime(...)
+- for counterparty in client.counterparties.list(created_at_upper_bound=dt.isoformat()):
++ for counterparty in client.counterparties.list(created_at_upper_bound=dt):
+  ...
+```
+
 ## Status
 
 This package is in beta. Its internals and interfaces are not stable and subject to change without a major semver bump;
 please reach out if you rely on any undocumented behavior.
 
 We are keen for your feedback; please email us at [sdk-feedback@moderntreasury.com](mailto:sdk-feedback@moderntreasury.com) or open an issue with questions,
 bugs, or suggestions.
 
 ## Requirements
 
-Python 3.7 or higher.
+Python 3.7 or higher.
```

