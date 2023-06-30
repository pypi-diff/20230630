# Comparing `tmp/gr4vy-0.12.0.tar.gz` & `tmp/gr4vy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gr4vy-0.12.0.tar", max compression
+gzip compressed data, was "gr4vy-0.2.0.tar", max compression
```

## Comparing `gr4vy-0.12.0.tar` & `gr4vy-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,254 @@
--rw-r--r--   0        0        0     1091 2023-04-12 15:27:03.763478 gr4vy-0.12.0/LICENSE
--rw-r--r--   0        0        0     4853 2023-06-28 15:52:10.361614 gr4vy-0.12.0/README.md
--rw-r--r--   0        0        0       62 2023-06-28 15:41:09.610010 gr4vy-0.12.0/gr4vy/__init__.py
--rw-r--r--   0        0        0    14660 2023-06-28 15:41:09.892654 gr4vy-0.12.0/gr4vy/gr4vy_client.py
--rw-r--r--   0        0        0     1418 2023-06-28 15:55:58.417286 gr4vy-0.12.0/pyproject.toml
--rw-r--r--   0        0        0     5767 1970-01-01 00:00:00.000000 gr4vy-0.12.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2021-12-17 15:53:35.135099 gr4vy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4760 2021-12-17 15:53:35.135357 gr4vy-0.2.0/README.md
+-rw-r--r--   0        0        0     1002 2021-12-17 15:53:35.135524 gr4vy-0.2.0/gr4vy/__init__.py
+-rw-r--r--   0        0        0    10581 2021-12-17 15:53:35.135907 gr4vy-0.2.0/gr4vy/gr4vy_api/.openapi-generator/FILES
+-rw-r--r--   0        0        0        5 2021-12-17 15:53:35.136007 gr4vy-0.2.0/gr4vy/gr4vy_api/.openapi-generator/VERSION
+-rw-r--r--   0        0        0     1040 2021-12-17 15:53:35.135692 gr4vy-0.2.0/gr4vy/gr4vy_api/.openapi-generator-ignore
+-rw-r--r--   0        0        0      940 2021-12-17 15:53:35.136331 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/__init__.py
+-rw-r--r--   0        0        0      233 2021-12-17 15:53:35.136498 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0    24104 2021-12-17 15:53:35.136795 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/buyers_api.py
+-rw-r--r--   0        0        0    23505 2021-12-17 15:53:35.136954 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/digital_wallets_api.py
+-rw-r--r--   0        0        0     5739 2021-12-17 15:53:35.137118 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/payment_method_tokens_api.py
+-rw-r--r--   0        0        0    25992 2021-12-17 15:53:35.137424 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/payment_methods_api.py
+-rw-r--r--   0        0        0     6526 2021-12-17 15:53:35.137579 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/payment_options_api.py
+-rw-r--r--   0        0        0    11140 2021-12-17 15:53:35.137692 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/payment_service_definitions_api.py
+-rw-r--r--   0        0        0    25268 2021-12-17 15:53:35.137851 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/payment_services_api.py
+-rw-r--r--   0        0        0    30006 2021-12-17 15:53:35.137998 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api/transactions_api.py
+-rw-r--r--   0        0        0    36889 2021-12-17 15:53:35.138338 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/api_client.py
+-rw-r--r--   0        0        0      977 2021-12-17 15:53:35.138508 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/apis/__init__.py
+-rw-r--r--   0        0        0    16778 2021-12-17 15:53:35.138694 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/configuration.py
+-rw-r--r--   0        0        0     1199 2021-12-17 15:53:35.139088 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Address.md
+-rw-r--r--   0        0        0     1302 2021-12-17 15:53:35.139212 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/AddressUpdate.md
+-rw-r--r--   0        0        0      618 2021-12-17 15:53:35.139311 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ApplePayRequest.md
+-rw-r--r--   0        0        0      543 2021-12-17 15:53:35.139407 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ApplePaySessionRequest.md
+-rw-r--r--   0        0        0      903 2021-12-17 15:53:35.139516 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/BillingDetails.md
+-rw-r--r--   0        0        0     1094 2021-12-17 15:53:35.139622 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/BillingDetailsUpdateRequest.md
+-rw-r--r--   0        0        0     1080 2021-12-17 15:53:35.139731 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Buyer.md
+-rw-r--r--   0        0        0      723 2021-12-17 15:53:35.139839 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/BuyerRequest.md
+-rw-r--r--   0        0        0      936 2021-12-17 15:53:35.139946 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/BuyerSnapshot.md
+-rw-r--r--   0        0        0      949 2021-12-17 15:53:35.140064 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/BuyerUpdate.md
+-rw-r--r--   0        0        0      936 2021-12-17 15:53:35.140155 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Buyers.md
+-rw-r--r--   0        0        0    16010 2021-12-17 15:53:35.140326 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/BuyersApi.md
+-rw-r--r--   0        0        0     1738 2021-12-17 15:53:35.140455 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/CardRequest.md
+-rw-r--r--   0        0        0     1300 2021-12-17 15:53:35.140566 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/DigitalWallet.md
+-rw-r--r--   0        0        0     1263 2021-12-17 15:53:35.140667 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/DigitalWalletRequest.md
+-rw-r--r--   0        0        0      767 2021-12-17 15:53:35.140764 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/DigitalWalletUpdate.md
+-rw-r--r--   0        0        0      437 2021-12-17 15:53:35.140876 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/DigitalWallets.md
+-rw-r--r--   0        0        0    15516 2021-12-17 15:53:35.140973 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/DigitalWalletsApi.md
+-rw-r--r--   0        0        0      930 2021-12-17 15:53:35.141071 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error400BadRequest.md
+-rw-r--r--   0        0        0      965 2021-12-17 15:53:35.141182 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error400IncorrectJson.md
+-rw-r--r--   0        0        0     1019 2021-12-17 15:53:35.141314 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error401Unauthorized.md
+-rw-r--r--   0        0        0      979 2021-12-17 15:53:35.141419 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error403Forbidden.md
+-rw-r--r--   0        0        0     1002 2021-12-17 15:53:35.141531 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error404NotFound.md
+-rw-r--r--   0        0        0     1026 2021-12-17 15:53:35.141617 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error404PendingCreation.md
+-rw-r--r--   0        0        0      966 2021-12-17 15:53:35.141699 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Error409DuplicateRecord.md
+-rw-r--r--   0        0        0      842 2021-12-17 15:53:35.141792 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ErrorDetail.md
+-rw-r--r--   0        0        0     1135 2021-12-17 15:53:35.141891 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ErrorGeneric.md
+-rw-r--r--   0        0        0     2074 2021-12-17 15:53:35.141974 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethod.md
+-rw-r--r--   0        0        0     2427 2021-12-17 15:53:35.142087 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodRequest.md
+-rw-r--r--   0        0        0     1477 2021-12-17 15:53:35.142195 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodSnapshot.md
+-rw-r--r--   0        0        0     1804 2021-12-17 15:53:35.142317 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodToken.md
+-rw-r--r--   0        0        0     1126 2021-12-17 15:53:35.142414 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodTokenized.md
+-rw-r--r--   0        0        0      460 2021-12-17 15:53:35.142521 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodTokens.md
+-rw-r--r--   0        0        0     3195 2021-12-17 15:53:35.142668 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodTokensApi.md
+-rw-r--r--   0        0        0      992 2021-12-17 15:53:35.142768 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethods.md
+-rw-r--r--   0        0        0    18094 2021-12-17 15:53:35.143082 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodsApi.md
+-rw-r--r--   0        0        0      488 2021-12-17 15:53:35.143200 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentMethodsTokenized.md
+-rw-r--r--   0        0        0     1102 2021-12-17 15:53:35.143306 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentOption.md
+-rw-r--r--   0        0        0      568 2021-12-17 15:53:35.143420 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentOptionContext.md
+-rw-r--r--   0        0        0      389 2021-12-17 15:53:35.143519 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentOptions.md
+-rw-r--r--   0        0        0     4158 2021-12-17 15:53:35.143643 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentOptionsApi.md
+-rw-r--r--   0        0        0     3149 2021-12-17 15:53:35.143777 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentService.md
+-rw-r--r--   0        0        0     1475 2021-12-17 15:53:35.143891 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceDefinition.md
+-rw-r--r--   0        0        0      775 2021-12-17 15:53:35.144004 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceDefinitionFields.md
+-rw-r--r--   0        0        0      808 2021-12-17 15:53:35.144111 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceDefinitionSupportedFeatures.md
+-rw-r--r--   0        0        0     1008 2021-12-17 15:53:35.144205 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceDefinitions.md
+-rw-r--r--   0        0        0     7259 2021-12-17 15:53:35.144302 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceDefinitionsApi.md
+-rw-r--r--   0        0        0     3174 2021-12-17 15:53:35.144383 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceRequest.md
+-rw-r--r--   0        0        0      403 2021-12-17 15:53:35.144480 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceRequestAllOf.md
+-rw-r--r--   0        0        0      709 2021-12-17 15:53:35.144574 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceSnapshot.md
+-rw-r--r--   0        0        0     2967 2021-12-17 15:53:35.144659 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceUpdate.md
+-rw-r--r--   0        0        0      529 2021-12-17 15:53:35.144751 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServiceUpdateFields.md
+-rw-r--r--   0        0        0      975 2021-12-17 15:53:35.144849 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServices.md
+-rw-r--r--   0        0        0    17553 2021-12-17 15:53:35.144997 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/PaymentServicesApi.md
+-rw-r--r--   0        0        0     1351 2021-12-17 15:53:35.145100 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/RedirectRequest.md
+-rw-r--r--   0        0        0      433 2021-12-17 15:53:35.145194 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ResetPasswordRequest.md
+-rw-r--r--   0        0        0      493 2021-12-17 15:53:35.145284 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/SetPasswordRequest.md
+-rw-r--r--   0        0        0      433 2021-12-17 15:53:35.145404 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TaxId.md
+-rw-r--r--   0        0        0      676 2021-12-17 15:53:35.145496 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ThreeDSecureData.md
+-rw-r--r--   0        0        0     1029 2021-12-17 15:53:35.145604 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ThreeDSecureDataV1.md
+-rw-r--r--   0        0        0      484 2021-12-17 15:53:35.145697 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ThreeDSecureDataV1AllOf.md
+-rw-r--r--   0        0        0     1156 2021-12-17 15:53:35.145784 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ThreeDSecureDataV1V2.md
+-rw-r--r--   0        0        0     1055 2021-12-17 15:53:35.145873 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ThreeDSecureDataV2.md
+-rw-r--r--   0        0        0      510 2021-12-17 15:53:35.145966 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/ThreeDSecureDataV2AllOf.md
+-rw-r--r--   0        0        0      963 2021-12-17 15:53:35.146082 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TokenizedRequest.md
+-rw-r--r--   0        0        0     2516 2021-12-17 15:53:35.146205 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Transaction.md
+-rw-r--r--   0        0        0      628 2021-12-17 15:53:35.146330 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionCaptureRequest.md
+-rw-r--r--   0        0        0     2103 2021-12-17 15:53:35.146430 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionPaymentMethodRequest.md
+-rw-r--r--   0        0        0      464 2021-12-17 15:53:35.146526 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionRefundRequest.md
+-rw-r--r--   0        0        0     2780 2021-12-17 15:53:35.146632 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionRequest.md
+-rw-r--r--   0        0        0     1754 2021-12-17 15:53:35.146741 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionSummary.md
+-rw-r--r--   0        0        0      966 2021-12-17 15:53:35.146832 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/Transactions.md
+-rw-r--r--   0        0        0    21632 2021-12-17 15:53:35.147018 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionsApi.md
+-rw-r--r--   0        0        0      768 2021-12-17 15:53:35.147131 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/TransactionsBatchCaptureRequest.md
+-rw-r--r--   0        0        0      643 2021-12-17 15:53:35.147209 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/docs/UserRequest.md
+-rw-r--r--   0        0        0     5134 2021-12-17 15:53:35.147303 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/exceptions.py
+-rw-r--r--   0        0        0      348 2021-12-17 15:53:35.147433 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/__init__.py
+-rw-r--r--   0        0        0     9306 2021-12-17 15:53:35.147662 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/address.py
+-rw-r--r--   0        0        0    11468 2021-12-17 15:53:35.147765 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/address_update.py
+-rw-r--r--   0        0        0     7167 2021-12-17 15:53:35.147892 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/apple_pay_request.py
+-rw-r--r--   0        0        0     6968 2021-12-17 15:53:35.148012 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/apple_pay_session_request.py
+-rw-r--r--   0        0        0     8343 2021-12-17 15:53:35.148169 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/billing_details.py
+-rw-r--r--   0        0        0    10378 2021-12-17 15:53:35.148360 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/billing_details_update_request.py
+-rw-r--r--   0        0        0     8396 2021-12-17 15:53:35.148494 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/buyer.py
+-rw-r--r--   0        0        0     7437 2021-12-17 15:53:35.148604 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/buyer_request.py
+-rw-r--r--   0        0        0     7859 2021-12-17 15:53:35.148720 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/buyer_snapshot.py
+-rw-r--r--   0        0        0     9584 2021-12-17 15:53:35.148833 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/buyer_update.py
+-rw-r--r--   0        0        0     7921 2021-12-17 15:53:35.148957 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/buyers.py
+-rw-r--r--   0        0        0     9569 2021-12-17 15:53:35.149088 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/card_request.py
+-rw-r--r--   0        0        0     8542 2021-12-17 15:53:35.149171 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/digital_wallet.py
+-rw-r--r--   0        0        0     8368 2021-12-17 15:53:35.149261 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/digital_wallet_request.py
+-rw-r--r--   0        0        0     7178 2021-12-17 15:53:35.149368 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/digital_wallet_update.py
+-rw-r--r--   0        0        0     6788 2021-12-17 15:53:35.149487 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/digital_wallets.py
+-rw-r--r--   0        0        0     7856 2021-12-17 15:53:35.149579 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error400_bad_request.py
+-rw-r--r--   0        0        0     7897 2021-12-17 15:53:35.149691 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error400_incorrect_json.py
+-rw-r--r--   0        0        0     8063 2021-12-17 15:53:35.149795 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error401_unauthorized.py
+-rw-r--r--   0        0        0     7989 2021-12-17 15:53:35.149904 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error403_forbidden.py
+-rw-r--r--   0        0        0     8035 2021-12-17 15:53:35.149998 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error404_not_found.py
+-rw-r--r--   0        0        0     8069 2021-12-17 15:53:35.150091 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error404_pending_creation.py
+-rw-r--r--   0        0        0     7896 2021-12-17 15:53:35.150185 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error409_duplicate_record.py
+-rw-r--r--   0        0        0     7458 2021-12-17 15:53:35.150281 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error_detail.py
+-rw-r--r--   0        0        0     8062 2021-12-17 15:53:35.150396 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/error_generic.py
+-rw-r--r--   0        0        0    10143 2021-12-17 15:53:35.150508 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_method.py
+-rw-r--r--   0        0        0    10224 2021-12-17 15:53:35.150611 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_method_request.py
+-rw-r--r--   0        0        0     8739 2021-12-17 15:53:35.150723 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_method_snapshot.py
+-rw-r--r--   0        0        0     8748 2021-12-17 15:53:35.150854 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_method_token.py
+-rw-r--r--   0        0        0     8734 2021-12-17 15:53:35.150975 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_method_tokenized.py
+-rw-r--r--   0        0        0     6836 2021-12-17 15:53:35.151086 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_method_tokens.py
+-rw-r--r--   0        0        0     8002 2021-12-17 15:53:35.151188 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_methods.py
+-rw-r--r--   0        0        0     6873 2021-12-17 15:53:35.151286 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_methods_tokenized.py
+-rw-r--r--   0        0        0     8228 2021-12-17 15:53:35.151387 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_option.py
+-rw-r--r--   0        0        0     7377 2021-12-17 15:53:35.151483 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_option_context.py
+-rw-r--r--   0        0        0     6749 2021-12-17 15:53:35.151571 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_options.py
+-rw-r--r--   0        0        0    13592 2021-12-17 15:53:35.151685 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service.py
+-rw-r--r--   0        0        0     9396 2021-12-17 15:53:35.151796 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_definition.py
+-rw-r--r--   0        0        0     7387 2021-12-17 15:53:35.151912 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_definition_fields.py
+-rw-r--r--   0        0        0     7505 2021-12-17 15:53:35.152001 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_definition_supported_features.py
+-rw-r--r--   0        0        0     8056 2021-12-17 15:53:35.152079 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_definitions.py
+-rw-r--r--   0        0        0    15404 2021-12-17 15:53:35.152154 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_request.py
+-rw-r--r--   0        0        0     6829 2021-12-17 15:53:35.152238 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_request_all_of.py
+-rw-r--r--   0        0        0     7567 2021-12-17 15:53:35.152322 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_snapshot.py
+-rw-r--r--   0        0        0    12478 2021-12-17 15:53:35.152397 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_update.py
+-rw-r--r--   0        0        0     6984 2021-12-17 15:53:35.152485 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_service_update_fields.py
+-rw-r--r--   0        0        0     7975 2021-12-17 15:53:35.152565 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/payment_services.py
+-rw-r--r--   0        0        0     8377 2021-12-17 15:53:35.152643 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/redirect_request.py
+-rw-r--r--   0        0        0     6647 2021-12-17 15:53:35.152731 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/reset_password_request.py
+-rw-r--r--   0        0        0     6909 2021-12-17 15:53:35.152802 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/set_password_request.py
+-rw-r--r--   0        0        0     8058 2021-12-17 15:53:35.152890 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/tax_id.py
+-rw-r--r--   0        0        0     7745 2021-12-17 15:53:35.152977 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/three_d_secure_data.py
+-rw-r--r--   0        0        0    10903 2021-12-17 15:53:35.153089 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/three_d_secure_data_v1.py
+-rw-r--r--   0        0        0     7288 2021-12-17 15:53:35.153178 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/three_d_secure_data_v1_all_of.py
+-rw-r--r--   0        0        0    11248 2021-12-17 15:53:35.153261 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/three_d_secure_data_v1_v2.py
+-rw-r--r--   0        0        0    10738 2021-12-17 15:53:35.153349 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/three_d_secure_data_v2.py
+-rw-r--r--   0        0        0     7125 2021-12-17 15:53:35.153432 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/three_d_secure_data_v2_all_of.py
+-rw-r--r--   0        0        0     7489 2021-12-17 15:53:35.153519 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/tokenized_request.py
+-rw-r--r--   0        0        0    12613 2021-12-17 15:53:35.153647 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transaction.py
+-rw-r--r--   0        0        0     6925 2021-12-17 15:53:35.153732 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transaction_capture_request.py
+-rw-r--r--   0        0        0     9817 2021-12-17 15:53:35.153819 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transaction_payment_method_request.py
+-rw-r--r--   0        0        0     6781 2021-12-17 15:53:35.153906 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transaction_refund_request.py
+-rw-r--r--   0        0        0    11162 2021-12-17 15:53:35.154020 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transaction_request.py
+-rw-r--r--   0        0        0    11013 2021-12-17 15:53:35.154095 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transaction_summary.py
+-rw-r--r--   0        0        0     7975 2021-12-17 15:53:35.154175 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transactions.py
+-rw-r--r--   0        0        0     7544 2021-12-17 15:53:35.154256 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/transactions_batch_capture_request.py
+-rw-r--r--   0        0        0     7183 2021-12-17 15:53:35.154332 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model/user_request.py
+-rw-r--r--   0        0        0    74841 2021-12-17 15:53:35.154751 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/model_utils.py
+-rw-r--r--   0        0        0     5281 2021-12-17 15:53:35.154921 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0    12583 2021-12-17 15:53:35.155038 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/rest.py
+-rw-r--r--   0        0        0        0 2021-12-17 15:53:35.155105 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/__init__.py
+-rw-r--r--   0        0        0      776 2021-12-17 15:53:35.155200 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_address.py
+-rw-r--r--   0        0        0      899 2021-12-17 15:53:35.155278 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_address_update.py
+-rw-r--r--   0        0        0      834 2021-12-17 15:53:35.155350 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_apple_pay_request.py
+-rw-r--r--   0        0        0      884 2021-12-17 15:53:35.155420 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_apple_pay_session_request.py
+-rw-r--r--   0        0        0      826 2021-12-17 15:53:35.155496 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_billing_details.py
+-rw-r--r--   0        0        0     1028 2021-12-17 15:53:35.155570 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_billing_details_update_request.py
+-rw-r--r--   0        0        0      762 2021-12-17 15:53:35.155640 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_buyer.py
+-rw-r--r--   0        0        0      812 2021-12-17 15:53:35.155702 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_buyer_request.py
+-rw-r--r--   0        0        0      819 2021-12-17 15:53:35.155764 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_buyer_snapshot.py
+-rw-r--r--   0        0        0      906 2021-12-17 15:53:35.155829 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_buyer_update.py
+-rw-r--r--   0        0        0      841 2021-12-17 15:53:35.155896 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_buyers.py
+-rw-r--r--   0        0        0     1272 2021-12-17 15:53:35.155958 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_buyers_api.py
+-rw-r--r--   0        0        0      805 2021-12-17 15:53:35.156020 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_card_request.py
+-rw-r--r--   0        0        0      819 2021-12-17 15:53:35.156084 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_digital_wallet.py
+-rw-r--r--   0        0        0      869 2021-12-17 15:53:35.156147 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_digital_wallet_request.py
+-rw-r--r--   0        0        0      862 2021-12-17 15:53:35.156208 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_digital_wallet_update.py
+-rw-r--r--   0        0        0      931 2021-12-17 15:53:35.156279 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_digital_wallets.py
+-rw-r--r--   0        0        0     1476 2021-12-17 15:53:35.156345 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_digital_wallets_api.py
+-rw-r--r--   0        0        0      952 2021-12-17 15:53:35.156411 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error400_bad_request.py
+-rw-r--r--   0        0        0      973 2021-12-17 15:53:35.156487 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error400_incorrect_json.py
+-rw-r--r--   0        0        0      965 2021-12-17 15:53:35.156567 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error401_unauthorized.py
+-rw-r--r--   0        0        0      944 2021-12-17 15:53:35.156637 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error403_forbidden.py
+-rw-r--r--   0        0        0      938 2021-12-17 15:53:35.156706 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error404_not_found.py
+-rw-r--r--   0        0        0      987 2021-12-17 15:53:35.156790 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error404_pending_creation.py
+-rw-r--r--   0        0        0      987 2021-12-17 15:53:35.156873 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error409_duplicate_record.py
+-rw-r--r--   0        0        0      805 2021-12-17 15:53:35.156956 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error_detail.py
+-rw-r--r--   0        0        0      909 2021-12-17 15:53:35.157058 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_error_generic.py
+-rw-r--r--   0        0        0      819 2021-12-17 15:53:35.157139 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method.py
+-rw-r--r--   0        0        0      869 2021-12-17 15:53:35.157223 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method_request.py
+-rw-r--r--   0        0        0      876 2021-12-17 15:53:35.157303 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method_snapshot.py
+-rw-r--r--   0        0        0      855 2021-12-17 15:53:35.157398 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method_token.py
+-rw-r--r--   0        0        0      883 2021-12-17 15:53:35.157485 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method_tokenized.py
+-rw-r--r--   0        0        0      988 2021-12-17 15:53:35.157580 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method_tokens.py
+-rw-r--r--   0        0        0      870 2021-12-17 15:53:35.157669 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_method_tokens_api.py
+-rw-r--r--   0        0        0      931 2021-12-17 15:53:35.157758 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_methods.py
+-rw-r--r--   0        0        0     1487 2021-12-17 15:53:35.157839 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_methods_api.py
+-rw-r--r--   0        0        0     1032 2021-12-17 15:53:35.157930 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_methods_tokenized.py
+-rw-r--r--   0        0        0      953 2021-12-17 15:53:35.158009 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_option.py
+-rw-r--r--   0        0        0      869 2021-12-17 15:53:35.158091 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_option_context.py
+-rw-r--r--   0        0        0      931 2021-12-17 15:53:35.158166 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_options.py
+-rw-r--r--   0        0        0      826 2021-12-17 15:53:35.158237 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_options_api.py
+-rw-r--r--   0        0        0      826 2021-12-17 15:53:35.158312 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service.py
+-rw-r--r--   0        0        0     1292 2021-12-17 15:53:35.158389 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_definition.py
+-rw-r--r--   0        0        0      940 2021-12-17 15:53:35.158465 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_definition_fields.py
+-rw-r--r--   0        0        0     1018 2021-12-17 15:53:35.158545 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_definition_supported_features.py
+-rw-r--r--   0        0        0     1054 2021-12-17 15:53:35.158623 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_definitions.py
+-rw-r--r--   0        0        0     1105 2021-12-17 15:53:35.158712 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_definitions_api.py
+-rw-r--r--   0        0        0     1329 2021-12-17 15:53:35.158799 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_request.py
+-rw-r--r--   0        0        0      913 2021-12-17 15:53:35.158915 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_request_all_of.py
+-rw-r--r--   0        0        0      883 2021-12-17 15:53:35.158992 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_snapshot.py
+-rw-r--r--   0        0        0     1028 2021-12-17 15:53:35.159063 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_update.py
+-rw-r--r--   0        0        0      912 2021-12-17 15:53:35.159142 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_service_update_fields.py
+-rw-r--r--   0        0        0      942 2021-12-17 15:53:35.159216 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_services.py
+-rw-r--r--   0        0        0     1468 2021-12-17 15:53:35.159291 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_payment_services_api.py
+-rw-r--r--   0        0        0      833 2021-12-17 15:53:35.159368 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_redirect_request.py
+-rw-r--r--   0        0        0      869 2021-12-17 15:53:35.159448 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_reset_password_request.py
+-rw-r--r--   0        0        0      855 2021-12-17 15:53:35.159536 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_set_password_request.py
+-rw-r--r--   0        0        0      763 2021-12-17 15:53:35.159611 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_tax_id.py
+-rw-r--r--   0        0        0      842 2021-12-17 15:53:35.159688 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_three_d_secure_data.py
+-rw-r--r--   0        0        0     1126 2021-12-17 15:53:35.159768 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_three_d_secure_data_v1.py
+-rw-r--r--   0        0        0      894 2021-12-17 15:53:35.159857 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_three_d_secure_data_v1_all_of.py
+-rw-r--r--   0        0        0     1128 2021-12-17 15:53:35.159942 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_three_d_secure_data_v1_v2.py
+-rw-r--r--   0        0        0     1126 2021-12-17 15:53:35.160020 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_three_d_secure_data_v2.py
+-rw-r--r--   0        0        0      894 2021-12-17 15:53:35.160092 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_three_d_secure_data_v2_all_of.py
+-rw-r--r--   0        0        0      840 2021-12-17 15:53:35.160168 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_tokenized_request.py
+-rw-r--r--   0        0        0      804 2021-12-17 15:53:35.160246 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transaction.py
+-rw-r--r--   0        0        0      904 2021-12-17 15:53:35.160323 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transaction_capture_request.py
+-rw-r--r--   0        0        0      947 2021-12-17 15:53:35.160403 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transaction_payment_method_request.py
+-rw-r--r--   0        0        0      897 2021-12-17 15:53:35.160478 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transaction_refund_request.py
+-rw-r--r--   0        0        0     1170 2021-12-17 15:53:35.160561 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transaction_request.py
+-rw-r--r--   0        0        0      854 2021-12-17 15:53:35.160643 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transaction_summary.py
+-rw-r--r--   0        0        0      907 2021-12-17 15:53:35.160710 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transactions.py
+-rw-r--r--   0        0        0     1424 2021-12-17 15:53:35.160780 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transactions_api.py
+-rw-r--r--   0        0        0      947 2021-12-17 15:53:35.160855 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_transactions_batch_capture_request.py
+-rw-r--r--   0        0        0      805 2021-12-17 15:53:35.160927 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client/test/test_user_request.py
+-rw-r--r--   0        0        0    13247 2021-12-17 15:53:35.161071 gr4vy-0.2.0/gr4vy/gr4vy_api/openapi_client_README.md
+-rw-r--r--   0        0        0     9449 2021-12-17 15:53:35.161180 gr4vy-0.2.0/gr4vy/gr4vy_client.py
+-rw-r--r--   0        0        0     1909 2021-12-17 15:53:35.161260 gr4vy-0.2.0/gr4vy/sdk_Buyers.py
+-rw-r--r--   0        0        0      726 2021-12-17 15:53:35.161335 gr4vy-0.2.0/gr4vy/sdk_PaymentMethodTokens.py
+-rw-r--r--   0        0        0     2631 2021-12-17 15:53:35.161432 gr4vy-0.2.0/gr4vy/sdk_PaymentMethods.py
+-rw-r--r--   0        0        0      860 2021-12-17 15:53:35.161499 gr4vy-0.2.0/gr4vy/sdk_PaymentOptions.py
+-rw-r--r--   0        0        0     1480 2021-12-17 15:53:35.161582 gr4vy-0.2.0/gr4vy/sdk_PaymentServiceDefinitions.py
+-rw-r--r--   0        0        0     2486 2021-12-17 15:53:35.161658 gr4vy-0.2.0/gr4vy/sdk_PaymentServices.py
+-rw-r--r--   0        0        0     2309 2021-12-17 15:53:35.161735 gr4vy-0.2.0/gr4vy/sdk_Transactions.py
+-rw-r--r--   0        0        0     1397 2021-12-17 15:54:23.064077 gr4vy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6171 2021-12-17 16:11:47.711433 gr4vy-0.2.0/setup.py
+-rw-r--r--   0        0        0     5580 2021-12-17 16:11:47.711767 gr4vy-0.2.0/PKG-INFO
```

### Comparing `gr4vy-0.12.0/LICENSE` & `gr4vy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gr4vy-0.12.0/pyproject.toml` & `gr4vy-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gr4vy"
-version = "0.12.0"
+version = "0.2.0"
 description = "Python SDK for Gr4vy"
 authors = ["Gr4vy <code@gr4vy.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 cryptography = "^3.4.6"
@@ -14,19 +14,18 @@
 PyJWT = "^2.3.0"
 pyOpenSSL = "^21.0.0"
 DateTime = "^4.3"
 six = "^1.16.0"
 urllib3 = "^1.26.5"
 python-dateutil="^2.8.2"
 pem = "^21.2.0"
-requests ="^2.28.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.1"
-black = "^22.3.0"
+black = "^21.6b0"
 pylint = "^2.9.3"
 rope = "^0.19.0"
 isort = "^5.9.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gr4vy-0.12.0/PKG-INFO` & `gr4vy-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: gr4vy
-Version: 0.12.0
+Version: 0.2.0
 Summary: Python SDK for Gr4vy
 Author: Gr4vy
 Author-email: code@gr4vy.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: DateTime (>=4.3,<5.0)
 Requires-Dist: PyJWT (>=2.3.0,<3.0.0)
 Requires-Dist: certifi (>=2021.10.8,<2022.0.0)
 Requires-Dist: cryptography (>=3.4.6,<4.0.0)
 Requires-Dist: pem (>=21.2.0,<22.0.0)
 Requires-Dist: pyOpenSSL (>=21.0.0,<22.0.0)
 Requires-Dist: pycryptodome (>=3.11.0,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.2.0,<4.0.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: urllib3 (>=1.26.5,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Gr4vy SDK for Python
 
 Gr4vy provides any of your payment integrations through one unified API. For
@@ -45,21 +43,21 @@
 ## Getting Started
 
 To make your first API call, you will need to [request](https://gr4vy.com) a
 Gr4vy instance to be set up. Please contact our sales team for a demo.
 
 Once you have been set up with a Gr4vy account you will need to head over to the
 **Integrations** panel and generate a private key. We recommend storing this key
-in a secure location but in this code sample, we simply read the file from disk.
-For multi-merchant environments, an optional merchant ID can be provided as well.
+in a secure location but in this code sample we simply read the file from disk.
 
 ```python
 from gr4vy import Gr4vyClient
-client = Gr4vyClient("gr4vy_instance","location_of_key_file", "sandbox_or_production", "my-merchant-id)
+client = Gr4vyClient("gr4vy_instance","location_of_key_file", "sandbox_or_production")
 client.ListBuyers()
+
 ```
 
 ## Gr4vy Embed
 
 To create a token for Gr4vy Embed, call the `client.GetEmbedToken(embed)`
 function with the amount, currency, and optional buyer information for Gr4vy
 Embed.
@@ -67,143 +65,141 @@
 ```python
 embed = {
   "amount": 1299,
   "currency": "USD",
   "buyerExternalIdentifier": "user-12345",
 }
 
-token = client.generate_embed_token(embed)
+token = client.GenerateEmbedToken(embed)
 ```
 
 You can now pass this token to your frontend where it can be used to
 authenticate Gr4vy Embed.
 
 The `buyer_id` and/or `buyer_external_identifier` fields can be used to allow
 the token to pull in previously stored payment methods for a user. A buyer
 needs to be created before it can be used in this way.
 
 ```python
   from gr4vy import Gr4vyClient
-
+  from gr4vy import BuyerRequest
   client = Gr4vyClient("gr4vy_instance","private_key.pem", "production")
 
-  buyer_request = {"display_name": "Jane Smith"}
-
-  new_buyer = client.create_new_buyer(**buyer_request).get('id')
-  embed_data = {
-    "amount": 1299,
-    "currency": "USD",
-    "buyerId": new_buyer,
-  }
-
-  embed_token = client.generate_embed_token(embed_data=embed_data)
+  buyer_request = BuyerRequest(display_name = "Jane Smith")
 
-  print("Embed token: {}".format(embed_token))
-```
-Checkout sessions can also be passed within an Embed token:
+  new_buyer = client.AddBuyer(buyer_request)
 
-```python
-  from gr4vy import Gr4vyClient
-
-  client = Gr4vyClient("gr4vy_instance","private_key.pem", "production")
-
-  checkout_session_id = client.create_new_checkout_session().get("id")
-  
-  embed_data = {
+  embed = {
     "amount": 1299,
     "currency": "USD",
+    "buyerId": new_buyer.id,
   }
 
-  emebed_token = client.generate_embed_token(
-        embed_data=embed_data, checkout_session_id=checkout_session_id
-    )
+  embed_token = client.GenerateEmbedToken(embed)
 
   print("Embed token: {}".format(embed_token))
 ```
 
-
-
 ## Initialization
 
 The client can be initialized with the Gr4vy ID (`gr4vyId`), the location of the private key, and the environment attempting to access.
 
 ```python
   client = Gr4vyClient("gr4vyId","private_key.pem", "sandbox")
 ```
 
 Alternatively, instead of the `gr4vyId` it can be initialized with the `baseUrl`
-of the server to use directly and the environment attempting to access.
+of the server to use directly and the environment attempting to acess .
 
 ```python
   client = Gr4vyClientWithBaseUrl("https://*gr4vyId*.gr4vy.app","private_key.pem", "sandbox")
 ```
 
 Your API private key can be created in your admin panel on the **Integrations**
 tab.
 
-## Multi Merchant
-Setting the Merchant ID for requests can be set on the client:
-
-```python
-  client = Gr4vyClient("gr4vyId","private_key.pem", "sandbox", merchant_account_id="merchant-id")
-```
 
 ## Making API calls
 
-This library conveniently maps every API path to a separate function. For
+This library conveniently maps every API path to a seperate function. For
 example, `GET /buyers?limit=100` would be:
 
 ```python
-  client.list_buyers({"limit=100"})
+  client.ListBuyers(2)
 ```
 
-To create, the API requires a request object for that resource. This is created by creating a dictionary object for the request.
+To create, the API requires a request object for that resource that is conventiently
+named `Gr4vy<Resource>Request`.  To update, the API requires a request object
+for that resource that is named `Gr4vy<Resource>Update`.
 
-For example, to create a buyer:
+For example, to create a buyer you will need to pass a `Gr4vyBuyerRequest` object to
+the `AddBuyer` method.
 
 ```python
   from gr4vy import BuyerRequest
 
-  buyer_request = {"display_name": "Jane Smith"}
-  new_buyer = client.add_buyer(**buyer_request)
+  buyer_request = BuyerRequest(display_name = "Jane Smith")
+  new_buyer = client.AddBuyer(buyer_request)
 
 ```
 
-To update a buyer:
+So to update a buyer you will need to pass in the `Gr4vyBuyerUpdate` to the
+`UpdateBuyer` method.
 
 ```python
-  buyer_id: "buyer_uuid_from_gr4vy"
-  buyer_request = {"display_name": "Jane Changed")
-  buyer_update = client.update_buyer(buyer_id, **buyer_request)
+  buyer_request = BuyerUpdate(display_name = "Jane Changed")
+  buyer_update = client.UpdateBuyer(buyer_id, buyer_request)
 ```
 
 ## Response
 
 Every resolved API call returns the requested resource, errors are printed to the console
 
 
 ```python
-  print(client.list_buyers())
+  print(client.ListBuyers())
 ```
 
 ## Logging & Debugging
 
-The SDK makes it possible to log responses to the console.
+The SDK makes it easy possible to log responses to the console.
 
 ```python
-  print(client.list_buyers())
+  print(client.ListBuyers())
 ```
 
 This will output the request parameters and response to the console as follows.
 
 ```sh
 {"items":[{"id":"b8433347-a16f-46b5-958f-d681876546a6","type":"buyer","display_name":"Jane Smith","external_identifier":None,"created_at":"2021-04-22T06:51:16.910297+00:00","updated_at":"2021-04-22T07:18:49.816242+00:00"}],"limit":1,"next_cursor":"fAA0YjY5NmU2My00NzY5LTQ2OGMtOTEyNC0xODVjMDdjZTY5MzEAMjAyMS0wNC0yMlQwNjozNTowNy4yNTMxMDY","previous_cursor":None}
 ```
 
+## Development
+
+### Adding new APIs
+
+To add new APIs, run the following command to update the models and APIs based
+on the API spec.
+
+```sh
+./openapi-generator-generate.sh
+```
+
+Run the tests to ensure the changes do not break any existing tests. Using PyTest. In `test_gr4vy.py` update the following lines with your Gr4vy ID and the location of the private key file.
+
+```python
+gr4vy_id = "YOUR_GR4VY_ID"
+private_key_location = "PRIVATE_KEY_LOCATION"
+```
+
+```sh
+pytest -v
+```
+
 ### Publishing
 
-This project is published on PyPi.
+This project is published to PyPi.
 
 ## License
 
 This library is released under the [MIT License](LICENSE).
```

