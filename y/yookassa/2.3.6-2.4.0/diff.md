# Comparing `tmp/yookassa-2.3.6.tar.gz` & `tmp/yookassa-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yookassa-2.3.6.tar", last modified: Mon May 22 11:58:41 2023, max compression
+gzip compressed data, was "yookassa-2.4.0.tar", last modified: Fri Jun 30 11:27:46 2023, max compression
```

## Comparing `yookassa-2.3.6.tar` & `yookassa-2.4.0.tar`

### file list

```diff
@@ -1,181 +1,184 @@
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.526081 yookassa-2.3.6/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1081 2023-05-22 11:58:40.000000 yookassa-2.3.6/LICENSE
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3235 2023-05-22 11:58:41.526184 yookassa-2.3.6/PKG-INFO
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6187 2023-05-22 11:58:40.000000 yookassa-2.3.6/README.md
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2023-05-22 11:58:41.527744 yookassa-2.3.6/setup.cfg
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3784 2023-05-22 11:58:40.000000 yookassa-2.3.6/setup.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.392109 yookassa-2.3.6/src/
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.402552 yookassa-2.3.6/src/yookassa/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      466 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3873 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/client.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2545 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/configuration.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1812 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/deal.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.406282 yookassa-2.3.6/src/yookassa/domain/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       88 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/__init__.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.416508 yookassa-2.3.6/src/yookassa/domain/common/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      858 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1490 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/base_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      553 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/confirmation_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/context.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      340 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/data_context.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      574 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/http_verb.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/payment_method_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      560 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/receipt_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      381 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/request_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      290 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/response_object.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      696 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/security_helper.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1097 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/type_factory.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3994 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/common/user_agent.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.424646 yookassa-2.3.6/src/yookassa/domain/exceptions/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      677 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/api_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      125 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/authorize_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/bad_request_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/forbidden_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      135 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/not_found_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      145 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/response_processing_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/too_many_request_error.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      139 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/exceptions/unauthorized_error.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.439741 yookassa-2.3.6/src/yookassa/domain/models/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1133 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4192 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/airline.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/amount.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1286 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/authorization_details.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1875 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/cancellation_details.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.443251 yookassa-2.3.6/src/yookassa/domain/models/confirmation/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      319 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2515 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      316 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.448811 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      550 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      551 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_external.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      922 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_qr.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      376 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_request.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.455058 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      901 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_external.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      794 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      864 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_qr.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1248 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      215 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/currency.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3800 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/deal.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.459284 yookassa-2.3.6/src/yookassa/domain/models/payment_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      518 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/card_type.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6794 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      366 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.474705 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1903 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      613 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      655 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2356 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      904 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_cash.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      970 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_installments.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      803 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      428 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      448 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      543 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.489590 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3572 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      629 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3397 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      921 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_cash.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      471 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_installments.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      819 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_psb.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      816 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      206 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.492777 yookassa-2.3.6/src/yookassa/domain/models/payout_data/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      328 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1403 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination_class_map.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      395 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination_factory.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.496748 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.500507 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2190 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/credit_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2333 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt_customer.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3518 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt_item.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      691 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/receipt_item_supplier.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/recipient.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1257 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/refund_source.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2772 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/requestor.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/settlement.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2088 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/models/transfer.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.502975 yookassa-2.3.6/src/yookassa/domain/notification/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      223 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/notification/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3976 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/notification/webhook_notification.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      468 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/notification/webhook_notification_types.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.514466 yookassa-2.3.6/src/yookassa/domain/request/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      745 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/capture_payment_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2631 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/capture_payment_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1605 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/deal_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      609 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/deal_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     9585 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payment_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1882 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payment_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3646 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payout_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/payout_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3377 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/receipt_item_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5606 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/receipt_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1124 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/receipt_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3499 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/refund_request.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      814 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/refund_request_builder.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/request/webhook_request.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.525863 yookassa-2.3.6/src/yookassa/domain/response/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      987 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/__init__.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      832 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/deal_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/deal_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/payment_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5333 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/payment_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2341 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/payout_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2040 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/receipt_item_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/receipt_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3575 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/receipt_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      838 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/refund_list_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2142 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/refund_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2076 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/transfer_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1062 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/domain/response/webhook_response.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3605 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/payment.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1611 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/payout.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1954 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/receipt.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1914 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/refund.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/settings.py
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1984 2023-05-22 11:58:40.000000 yookassa-2.3.6/src/yookassa/webhook.py
-drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-05-22 11:58:41.405750 yookassa-2.3.6/src/yookassa.egg-info/
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3235 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/PKG-INFO
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     8658 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/not-zip-safe
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       43 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/requires.txt
--rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        9 2023-05-22 11:58:41.000000 yookassa-2.3.6/src/yookassa.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.076972 yookassa-2.4.0/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1081 2023-06-30 11:27:44.000000 yookassa-2.4.0/LICENSE
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3235 2023-06-30 11:27:46.077059 yookassa-2.4.0/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6187 2023-06-30 11:27:44.000000 yookassa-2.4.0/README.md
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       97 2023-06-30 11:27:46.078090 yookassa-2.4.0/setup.cfg
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3784 2023-06-30 11:27:44.000000 yookassa-2.4.0/setup.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.949660 yookassa-2.4.0/src/
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.964674 yookassa-2.4.0/src/yookassa/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      466 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3873 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/client.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2545 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/configuration.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1812 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/deal.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.970260 yookassa-2.4.0/src/yookassa/domain/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       88 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/__init__.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.980012 yookassa-2.4.0/src/yookassa/domain/common/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      858 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1490 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/base_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      553 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/confirmation_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      386 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      340 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/data_context.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      574 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/http_verb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1626 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/payment_method_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      560 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/receipt_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      381 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/request_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      290 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/response_object.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      696 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/security_helper.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1097 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/type_factory.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3994 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/common/user_agent.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.986228 yookassa-2.4.0/src/yookassa/domain/exceptions/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      677 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       62 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/api_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      125 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/authorize_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/bad_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      137 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/forbidden_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      135 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/not_found_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      145 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/response_processing_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      142 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/too_many_request_error.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      139 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/exceptions/unauthorized_error.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.999000 yookassa-2.4.0/src/yookassa/domain/models/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1133 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     4192 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/airline.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/amount.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1286 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/authorization_details.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1875 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/cancellation_details.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.002095 yookassa-2.4.0/src/yookassa/domain/models/confirmation/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      319 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/confirmation.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2515 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/confirmation_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      316 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/confirmation_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.007328 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      550 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      551 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_external.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      922 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_qr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      376 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.011774 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      901 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      521 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_external.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      794 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      864 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_qr.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1248 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      215 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/currency.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3800 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/deal.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.015767 yookassa-2.4.0/src/yookassa/domain/models/payment_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      518 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/card_type.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/payment_data.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     6809 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/payment_data_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      366 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/payment_data_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.028788 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1903 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      613 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      655 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2356 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      904 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_cash.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      970 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_installments.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      803 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      765 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      450 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_sber_loan.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      428 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      448 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      543 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      462 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.047684 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3572 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      629 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_applepay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3397 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      921 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_cash.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      471 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_installments.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      819 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_psb.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      781 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1331 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_sber_loan.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      816 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      460 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_unknown.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      464 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      478 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      206 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.050377 yookassa-2.4.0/src/yookassa/domain/models/payout_data/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      328 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/payout_destination.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1403 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/payout_destination_class_map.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      395 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/payout_destination_factory.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.053342 yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      444 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.055558 yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2190 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/credit_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      940 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      711 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2333 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1052 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/receipt_customer.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3518 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/receipt_item.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      691 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/receipt_item_supplier.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      559 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/recipient.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1257 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/refund_source.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2772 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/requestor.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/settlement.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2088 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/models/transfer.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.058679 yookassa-2.4.0/src/yookassa/domain/notification/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      223 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/notification/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3976 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/notification/webhook_notification.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      468 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/notification/webhook_notification_types.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.068623 yookassa-2.4.0/src/yookassa/domain/request/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1121 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      745 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/capture_payment_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2631 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/capture_payment_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1605 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/deal_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      609 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/deal_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     9585 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/payment_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1882 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/payment_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3646 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/payout_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      837 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/payout_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3377 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/receipt_item_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5606 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/receipt_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1124 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/receipt_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3499 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/refund_request.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      814 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/refund_request_builder.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      508 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/request/webhook_request.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:46.076759 yookassa-2.4.0/src/yookassa/domain/response/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      987 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/__init__.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      832 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/deal_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2066 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/deal_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/payment_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     5609 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/payment_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2341 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/payout_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2040 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/receipt_item_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      844 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/receipt_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3575 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/receipt_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      838 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/refund_list_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2142 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/refund_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     2076 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/transfer_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1062 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/domain/response/webhook_response.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3661 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/payment.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1611 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/payout.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1954 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/receipt.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1914 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/refund.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)      670 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/settings.py
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     1984 2023-06-30 11:27:44.000000 yookassa-2.4.0/src/yookassa/webhook.py
+drwxr-xr-x   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        0 2023-06-30 11:27:45.969379 yookassa-2.4.0/src/yookassa.egg-info/
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     3235 2023-06-30 11:27:45.000000 yookassa-2.4.0/src/yookassa.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)     8880 2023-06-30 11:27:45.000000 yookassa-2.4.0/src/yookassa.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-06-30 11:27:45.000000 yookassa-2.4.0/src/yookassa.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        1 2023-06-30 11:27:45.000000 yookassa-2.4.0/src/yookassa.egg-info/not-zip-safe
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)       43 2023-06-30 11:27:45.000000 yookassa-2.4.0/src/yookassa.egg-info/requires.txt
+-rw-r--r--   0 nikolaevanym (494676782) YAMONEY\Пользователи домена (585421731)        9 2023-06-30 11:27:45.000000 yookassa-2.4.0/src/yookassa.egg-info/top_level.txt
```

### Comparing `yookassa-2.3.6/LICENSE` & `yookassa-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/PKG-INFO` & `yookassa-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yookassa
-Version: 2.3.6
+Version: 2.4.0
 Summary: YooKassa API SDK Python Library
 Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
 Author: YooMoney
 Author-email: cms@yoomoney.ru
 License: MIT
 Keywords: yoomoney,yookassa,payout,sdk,python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yookassa-2.3.6/README.md` & `yookassa-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/setup.py` & `yookassa-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/client.py` & `yookassa-2.4.0/src/yookassa/client.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/configuration.py` & `yookassa-2.4.0/src/yookassa/configuration.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/deal.py` & `yookassa-2.4.0/src/yookassa/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/__init__.py` & `yookassa-2.4.0/src/yookassa/domain/common/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/base_object.py` & `yookassa-2.4.0/src/yookassa/domain/common/base_object.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/confirmation_type.py` & `yookassa-2.4.0/src/yookassa/domain/common/confirmation_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/http_verb.py` & `yookassa-2.4.0/src/yookassa/domain/common/http_verb.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/payment_method_type.py` & `yookassa-2.4.0/src/yookassa/domain/common/payment_method_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     * yookassa.domain.common.PaymentMethodType.APPLEPAY
     * yookassa.domain.common.PaymentMethodType.GOOGLE_PAY
     * yookassa.domain.common.PaymentMethodType.INSTALMENTS
     * yookassa.domain.common.PaymentMethodType.B2B_SBERBANK
     * yookassa.domain.common.PaymentMethodType.TINKOFF_BANK
     * yookassa.domain.common.PaymentMethodType.WECHAT
     * yookassa.domain.common.PaymentMethodType.SBP
+    * yookassa.domain.common.PaymentMethodType.SBER_LOAN
+    * yookassa.domain.common.PaymentMethodType.UNKNOWN
     """
     YOO_MONEY = 'yoo_money'
     BANK_CARD = 'bank_card'
     SBERBANK = 'sberbank'
     CASH = 'cash'
     MOBILE_BALANCE = 'mobile_balance'
     PSB = 'psb'
@@ -34,7 +36,9 @@
     APPLEPAY = 'apple_pay'
     GOOGLE_PAY = 'google_pay'
     INSTALMENTS = 'installments'
     B2B_SBERBANK = 'b2b_sberbank'
     TINKOFF_BANK = 'tinkoff_bank'
     WECHAT = 'wechat'
     SBP = 'sbp'
+    SBER_LOAN = 'sber_loan'
+    UNKNOWN = 'unknown'
```

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/receipt_type.py` & `yookassa-2.4.0/src/yookassa/domain/common/receipt_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/security_helper.py` & `yookassa-2.4.0/src/yookassa/domain/common/security_helper.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/type_factory.py` & `yookassa-2.4.0/src/yookassa/domain/common/type_factory.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/common/user_agent.py` & `yookassa-2.4.0/src/yookassa/domain/common/user_agent.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/exceptions/__init__.py` & `yookassa-2.4.0/src/yookassa/domain/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/__init__.py` & `yookassa-2.4.0/src/yookassa/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/airline.py` & `yookassa-2.4.0/src/yookassa/domain/models/airline.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/amount.py` & `yookassa-2.4.0/src/yookassa/domain/models/amount.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/authorization_details.py` & `yookassa-2.4.0/src/yookassa/domain/models/authorization_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/cancellation_details.py` & `yookassa-2.4.0/src/yookassa/domain/models/cancellation_details.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/confirmation_class_map.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/confirmation_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_external.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_qr.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/request/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_embedded.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_external.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_external.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_mobile_application.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_qr.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_qr.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py` & `yookassa-2.4.0/src/yookassa/domain/models/confirmation/response/confirmation_redirect.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/deal.py` & `yookassa-2.4.0/src/yookassa/domain/models/deal.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/card_type.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/card_type.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/payment_data.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/payment_data_class_map.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/payment_data_class_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 from yookassa.domain.common.data_context import DataContext
 from yookassa.domain.common.payment_method_type import PaymentMethodType
-from yookassa.domain.models.payment_data.request.payment_data_alfabank import \
-    PaymentDataAlfabank as RequestPaymentDataAlfabank
 from yookassa.domain.models.payment_data.request.payment_data_applepay import \
     PaymentDataApplepay as RequestPaymentDataApplepay
 from yookassa.domain.models.payment_data.request.payment_data_b2b_sberbank import \
     PaymentDataB2bSberbank as RequestPaymentDataB2bSberbank
 from yookassa.domain.models.payment_data.request.payment_data_bank_card import \
     PaymentDataBankCard as RequestPaymentDataBankCard
 from yookassa.domain.models.payment_data.request.payment_data_cash import \
@@ -19,22 +17,20 @@
     PaymentDataMobileBalance as RequestPaymentDataMobileBalance
 from yookassa.domain.models.payment_data.request.payment_data_qiwi import \
     PaymentDataQiwi as RequestPaymentDataQiwi
 from yookassa.domain.models.payment_data.request.payment_data_sberbank import \
     PaymentDataSberbank as RequestPaymentDataSberbank
 from yookassa.domain.models.payment_data.request.payment_data_tinkoff_bank import \
     PaymentDataTinkoffBank as RequestPaymentDataTinkoffBank
-from yookassa.domain.models.payment_data.request.payment_data_webmoney import \
-    PaymentDataWebmoney as RequestPaymentDataWebmoney
-from yookassa.domain.models.payment_data.request.payment_data_wechat import \
-    PaymentDataWechat as RequestPaymentDataWechat
 from yookassa.domain.models.payment_data.request.payment_data_yoomoney_wallet import \
     PaymentDataYooMoneyWallet as RequestPaymentDataYooMoneyWallet
 from yookassa.domain.models.payment_data.request.payment_data_sbp import \
     PaymentDataSbp as RequestPaymentDataSbp
+from yookassa.domain.models.payment_data.request.payment_data_sber_loan import \
+    PaymentDataSberLoan as RequestPaymentDataSberLoan
 from yookassa.domain.models.payment_data.response.payment_data_alfabank import \
     PaymentDataAlfabank as ResponsePaymentDataAlfabank
 from yookassa.domain.models.payment_data.response.payment_data_applepay import \
     PaymentDataApplepay as ResponsePaymentDataApplepay
 from yookassa.domain.models.payment_data.response.payment_data_b2b_sberbank import \
     PaymentDataB2bSberbank as ResponsePaymentDataB2bSberbank
 from yookassa.domain.models.payment_data.response.payment_data_bank_card import \
@@ -59,38 +55,40 @@
     PaymentDataWebmoney as ResponsePaymentDataWebmoney
 from yookassa.domain.models.payment_data.response.payment_data_wechat import \
     PaymentDataWechat as ResponsePaymentDataWechat
 from yookassa.domain.models.payment_data.response.payment_data_yoomoney_wallet import \
     PaymentDataYooMoneyWallet as ResponsePaymentDataYooMoneyWallet
 from yookassa.domain.models.payment_data.response.payment_data_sbp import \
     PaymentDataSbp as ResponsePaymentDataSbp
+from yookassa.domain.models.payment_data.response.payment_data_sber_loan import \
+    PaymentDataSberLoan as ResponsePaymentDataSberLoan
+from yookassa.domain.models.payment_data.response.payment_data_unknown import \
+    PaymentDataUnknown as ResponsePaymentDataUnknown
 
 
 class PaymentDataClassMap(DataContext):
     def __init__(self):
         super(PaymentDataClassMap, self).__init__(('request', 'response'))
 
     @property
     def request(self):
         return {
-            PaymentMethodType.ALFABANK: RequestPaymentDataAlfabank,
             PaymentMethodType.BANK_CARD: RequestPaymentDataBankCard,
             PaymentMethodType.CASH: RequestPaymentDataCash,
             PaymentMethodType.MOBILE_BALANCE: RequestPaymentDataMobileBalance,
             PaymentMethodType.SBERBANK: RequestPaymentDataSberbank,
             PaymentMethodType.YOO_MONEY: RequestPaymentDataYooMoneyWallet,
             PaymentMethodType.QIWI: RequestPaymentDataQiwi,
-            PaymentMethodType.WEBMONEY: RequestPaymentDataWebmoney,
             PaymentMethodType.APPLEPAY: RequestPaymentDataApplepay,
             PaymentMethodType.GOOGLE_PAY: RequestPaymentDataGooglePay,
             PaymentMethodType.INSTALMENTS: RequestPaymentDataInstallments,
             PaymentMethodType.B2B_SBERBANK: RequestPaymentDataB2bSberbank,
             PaymentMethodType.TINKOFF_BANK: RequestPaymentDataTinkoffBank,
-            PaymentMethodType.WECHAT: RequestPaymentDataWechat,
             PaymentMethodType.SBP: RequestPaymentDataSbp,
+            PaymentMethodType.SBER_LOAN: RequestPaymentDataSberLoan,
         }
 
     @property
     def response(self):
         return {
             PaymentMethodType.ALFABANK: ResponsePaymentDataAlfabank,
             PaymentMethodType.BANK_CARD: ResponsePaymentDataBankCard,
@@ -104,8 +102,10 @@
             PaymentMethodType.APPLEPAY: ResponsePaymentDataApplepay,
             PaymentMethodType.GOOGLE_PAY: ResponsePaymentDataGooglePay,
             PaymentMethodType.INSTALMENTS: ResponsePaymentDataInstallments,
             PaymentMethodType.B2B_SBERBANK: ResponsePaymentDataB2bSberbank,
             PaymentMethodType.TINKOFF_BANK: ResponsePaymentDataTinkoffBank,
             PaymentMethodType.WECHAT: ResponsePaymentDataWechat,
             PaymentMethodType.SBP: ResponsePaymentDataSbp,
+            PaymentMethodType.SBER_LOAN: ResponsePaymentDataSberLoan,
+            PaymentMethodType.UNKNOWN: ResponsePaymentDataUnknown,
         }
```

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/credit_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_alfabank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_applepay.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_cash.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/request/payment_data_wechat.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/credit_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_alfabank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_b2b_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_cash.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_cash.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py` & `yookassa-2.4.0/src/yookassa/domain/models/payment_data/response/payment_data_wechat.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payout_data/payout_destination_class_map.py` & `yookassa-2.4.0/src/yookassa/domain/models/payout_data/payout_destination_class_map.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py` & `yookassa-2.4.0/src/yookassa/domain/models/payout_data/request/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/credit_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/credit_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py` & `yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/payout_destination_bank_card.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py` & `yookassa-2.4.0/src/yookassa/domain/models/payout_data/response/payout_destination_yoomoney_wallet.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/receipt.py` & `yookassa-2.4.0/src/yookassa/domain/models/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/receipt_customer.py` & `yookassa-2.4.0/src/yookassa/domain/models/receipt_customer.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/receipt_item.py` & `yookassa-2.4.0/src/yookassa/domain/models/receipt_item.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/receipt_item_supplier.py` & `yookassa-2.4.0/src/yookassa/domain/models/receipt_item_supplier.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/recipient.py` & `yookassa-2.4.0/src/yookassa/domain/models/recipient.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/refund_source.py` & `yookassa-2.4.0/src/yookassa/domain/models/refund_source.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/requestor.py` & `yookassa-2.4.0/src/yookassa/domain/models/requestor.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/settlement.py` & `yookassa-2.4.0/src/yookassa/domain/models/settlement.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/models/transfer.py` & `yookassa-2.4.0/src/yookassa/domain/models/transfer.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/notification/webhook_notification.py` & `yookassa-2.4.0/src/yookassa/domain/notification/webhook_notification.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/__init__.py` & `yookassa-2.4.0/src/yookassa/domain/request/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/capture_payment_builder.py` & `yookassa-2.4.0/src/yookassa/domain/request/capture_payment_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/capture_payment_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/capture_payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/deal_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/deal_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/deal_request_builder.py` & `yookassa-2.4.0/src/yookassa/domain/request/deal_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/payment_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/payment_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/payment_request_builder.py` & `yookassa-2.4.0/src/yookassa/domain/request/payment_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/payout_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/payout_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/payout_request_builder.py` & `yookassa-2.4.0/src/yookassa/domain/request/payout_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/receipt_item_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/receipt_item_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/receipt_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/receipt_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/receipt_request_builder.py` & `yookassa-2.4.0/src/yookassa/domain/request/receipt_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/refund_request.py` & `yookassa-2.4.0/src/yookassa/domain/request/refund_request.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/request/refund_request_builder.py` & `yookassa-2.4.0/src/yookassa/domain/request/refund_request_builder.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/__init__.py` & `yookassa-2.4.0/src/yookassa/domain/response/__init__.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/deal_list_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/deal_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/deal_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/deal_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/payment_list_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/payment_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/payment_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/payment_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
-from yookassa.domain.common import ResponseObject
+from yookassa.domain.common import ResponseObject, PaymentMethodType
 from yookassa.domain.models import Amount, AuthorizationDetails, CancellationDetails, Recipient
 from yookassa.domain.models.confirmation.confirmation_factory import ConfirmationFactory
 from yookassa.domain.models.deal import PaymentDealInfo
+from yookassa.domain.models.payment_data.payment_data_class_map import PaymentDataClassMap
 from yookassa.domain.models.payment_data.payment_data_factory import PaymentDataFactory
 from yookassa.domain.response.transfer_response import TransferResponse
 
 
 class PaymentResponse(ResponseObject):
     """
     Class representing response object.
@@ -107,14 +108,16 @@
 
     @property
     def payment_method(self):
         return self.__payment_method
 
     @payment_method.setter
     def payment_method(self, value):
+        if isinstance(value, dict) and 'type' in value and value['type'] not in PaymentDataClassMap().response:
+            value['type'] = PaymentMethodType.UNKNOWN
         self.__payment_method = PaymentDataFactory().create(value, self.context())
 
     @property
     def captured_at(self):
         return self.__captured_at
 
     @captured_at.setter
```

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/payout_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/payout_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/receipt_item_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/receipt_item_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/receipt_list_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/receipt_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/receipt_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/receipt_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/refund_list_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/refund_list_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/refund_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/refund_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/transfer_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/transfer_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/domain/response/webhook_response.py` & `yookassa-2.4.0/src/yookassa/domain/response/webhook_response.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/payment.py` & `yookassa-2.4.0/src/yookassa/payment.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,13 +111,15 @@
         headers = {
             'Idempotence-Key': str(idempotency_key)
         }
         response = instance.client.request(HttpVerb.POST, path, None, headers)
         return PaymentResponse(response)
 
     @classmethod
-    def list(cls, params):
+    def list(cls, params=None):
+        if params is None:
+            params = {}
         instance = cls()
         path = cls.base_path
 
         response = instance.client.request(HttpVerb.GET, path, params)
         return PaymentListResponse(response)
```

### Comparing `yookassa-2.3.6/src/yookassa/payout.py` & `yookassa-2.4.0/src/yookassa/payout.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/receipt.py` & `yookassa-2.4.0/src/yookassa/receipt.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/refund.py` & `yookassa-2.4.0/src/yookassa/refund.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/settings.py` & `yookassa-2.4.0/src/yookassa/settings.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa/webhook.py` & `yookassa-2.4.0/src/yookassa/webhook.py`

 * *Files identical despite different names*

### Comparing `yookassa-2.3.6/src/yookassa.egg-info/PKG-INFO` & `yookassa-2.4.0/src/yookassa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yookassa
-Version: 2.3.6
+Version: 2.4.0
 Summary: YooKassa API SDK Python Library
 Home-page: https://git.yoomoney.ru/projects/SDK/repos/yookassa-sdk-python
 Author: YooMoney
 Author-email: cms@yoomoney.ru
 License: MIT
 Keywords: yoomoney,yookassa,payout,sdk,python
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yookassa-2.3.6/src/yookassa.egg-info/SOURCES.txt` & `yookassa-2.4.0/src/yookassa.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 src/yookassa/domain/models/payment_data/request/payment_data_b2b_sberbank.py
 src/yookassa/domain/models/payment_data/request/payment_data_bank_card.py
 src/yookassa/domain/models/payment_data/request/payment_data_cash.py
 src/yookassa/domain/models/payment_data/request/payment_data_google_pay.py
 src/yookassa/domain/models/payment_data/request/payment_data_installments.py
 src/yookassa/domain/models/payment_data/request/payment_data_mobile_balance.py
 src/yookassa/domain/models/payment_data/request/payment_data_qiwi.py
+src/yookassa/domain/models/payment_data/request/payment_data_sber_loan.py
 src/yookassa/domain/models/payment_data/request/payment_data_sberbank.py
 src/yookassa/domain/models/payment_data/request/payment_data_sbp.py
 src/yookassa/domain/models/payment_data/request/payment_data_tinkoff_bank.py
 src/yookassa/domain/models/payment_data/request/payment_data_webmoney.py
 src/yookassa/domain/models/payment_data/request/payment_data_wechat.py
 src/yookassa/domain/models/payment_data/request/payment_data_yoomoney_wallet.py
 src/yookassa/domain/models/payment_data/response/__init__.py
@@ -105,17 +106,19 @@
 src/yookassa/domain/models/payment_data/response/payment_data_bank_card.py
 src/yookassa/domain/models/payment_data/response/payment_data_cash.py
 src/yookassa/domain/models/payment_data/response/payment_data_google_pay.py
 src/yookassa/domain/models/payment_data/response/payment_data_installments.py
 src/yookassa/domain/models/payment_data/response/payment_data_mobile_balance.py
 src/yookassa/domain/models/payment_data/response/payment_data_psb.py
 src/yookassa/domain/models/payment_data/response/payment_data_qiwi.py
+src/yookassa/domain/models/payment_data/response/payment_data_sber_loan.py
 src/yookassa/domain/models/payment_data/response/payment_data_sberbank.py
 src/yookassa/domain/models/payment_data/response/payment_data_sbp.py
 src/yookassa/domain/models/payment_data/response/payment_data_tinkoff_bank.py
+src/yookassa/domain/models/payment_data/response/payment_data_unknown.py
 src/yookassa/domain/models/payment_data/response/payment_data_webmoney.py
 src/yookassa/domain/models/payment_data/response/payment_data_wechat.py
 src/yookassa/domain/models/payment_data/response/payment_data_yoomoney_wallet.py
 src/yookassa/domain/models/payout_data/__init__.py
 src/yookassa/domain/models/payout_data/payout_destination.py
 src/yookassa/domain/models/payout_data/payout_destination_class_map.py
 src/yookassa/domain/models/payout_data/payout_destination_factory.py
```

