# Comparing `tmp/stigg_api_client_v2-0.468.0.tar.gz` & `tmp/stigg_api_client_v2-0.470.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.468.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.470.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.468.0.tar` & `stigg_api_client_v2-0.470.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1644 2023-06-26 16:35:37.998444 stigg_api_client_v2-0.468.0/README.md
--rw-r--r--   0        0        0      653 2023-06-26 16:36:16.654441 stigg_api_client_v2-0.468.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-06-26 16:35:37.998444 stigg_api_client_v2-0.468.0/stigg/__init__.py
--rw-r--r--   0        0        0      363 2023-06-26 16:35:37.998444 stigg_api_client_v2-0.468.0/stigg/client.py
--rw-r--r--   0        0        0    39681 2023-06-26 16:36:15.026442 stigg_api_client_v2-0.468.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0     7303 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0     1951 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-06-26 16:36:13.826442 stigg_api_client_v2-0.468.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-06-26 16:36:13.842442 stigg_api_client_v2-0.468.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    70260 2023-06-26 16:36:14.878442 stigg_api_client_v2-0.468.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-06-26 16:36:13.866442 stigg_api_client_v2-0.468.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0      541 2023-06-26 16:36:13.950442 stigg_api_client_v2-0.468.0/stigg/generated/entitlements_updated.py
--rw-r--r--   0        0        0    23994 2023-06-26 16:36:11.658443 stigg_api_client_v2-0.468.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-06-26 16:36:13.830442 stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-06-26 16:36:13.838442 stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    53605 2023-06-26 16:36:14.666442 stigg_api_client_v2-0.468.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-06-26 16:36:13.886442 stigg_api_client_v2-0.468.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-06-26 16:36:13.894442 stigg_api_client_v2-0.468.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-06-26 16:36:13.878442 stigg_api_client_v2-0.468.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-06-26 16:36:13.930442 stigg_api_client_v2-0.468.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-06-26 16:36:13.910442 stigg_api_client_v2-0.468.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-06-26 16:36:13.902442 stigg_api_client_v2-0.468.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-06-26 16:36:13.938442 stigg_api_client_v2-0.468.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-06-26 16:36:13.898442 stigg_api_client_v2-0.468.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-06-26 16:36:13.918442 stigg_api_client_v2-0.468.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-06-26 16:36:13.926442 stigg_api_client_v2-0.468.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-06-26 16:36:13.794442 stigg_api_client_v2-0.468.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-06-26 16:36:13.786442 stigg_api_client_v2-0.468.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-06-26 16:36:13.814442 stigg_api_client_v2-0.468.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126193 2023-06-26 16:36:13.770442 stigg_api_client_v2-0.468.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-06-26 16:36:13.870442 stigg_api_client_v2-0.468.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-06-26 16:36:13.782442 stigg_api_client_v2-0.468.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-06-26 16:36:13.806442 stigg_api_client_v2-0.468.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-06-26 16:36:13.858442 stigg_api_client_v2-0.468.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-06-26 16:36:13.854442 stigg_api_client_v2-0.468.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-06-26 16:36:13.850442 stigg_api_client_v2-0.468.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-06-26 16:36:14.670442 stigg_api_client_v2-0.468.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-06-26 16:36:13.798442 stigg_api_client_v2-0.468.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-06-26 16:36:13.818442 stigg_api_client_v2-0.468.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-06-26 16:36:13.946442 stigg_api_client_v2-0.468.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0      451 2023-06-26 16:36:13.958442 stigg_api_client_v2-0.468.0/stigg/generated/usage_updated.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.468.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-06-12 16:19:38.768385 stigg_api_client_v2-0.470.0/README.md
+-rw-r--r--   0        0        0      432 2023-06-30 16:55:06.815193 stigg_api_client_v2-0.470.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-06-30 16:39:54.462400 stigg_api_client_v2-0.470.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-30 16:39:54.462736 stigg_api_client_v2-0.470.0/stigg/client.py
+-rw-r--r--   0        0        0    39399 2023-06-30 16:23:24.123748 stigg_api_client_v2-0.470.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0     7303 2023-06-30 16:23:23.230934 stigg_api_client_v2-0.470.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    66201 2023-06-30 16:23:23.754796 stigg_api_client_v2-0.470.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-06-30 16:23:14.372387 stigg_api_client_v2-0.470.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-06-30 16:23:23.232149 stigg_api_client_v2-0.470.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-06-30 16:23:21.569815 stigg_api_client_v2-0.470.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-06-30 16:23:21.598608 stigg_api_client_v2-0.470.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    65786 2023-06-30 16:23:14.852597 stigg_api_client_v2-0.470.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-06-30 16:23:21.639459 stigg_api_client_v2-0.470.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    23994 2023-06-30 16:23:16.926481 stigg_api_client_v2-0.470.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-06-30 16:23:21.580409 stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-06-30 16:23:21.592114 stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-06-30 16:23:23.232391 stigg_api_client_v2-0.470.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    53605 2023-06-30 16:23:23.229439 stigg_api_client_v2-0.470.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-06-30 16:23:21.676317 stigg_api_client_v2-0.470.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-06-30 16:23:21.693093 stigg_api_client_v2-0.470.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-06-30 16:23:21.663635 stigg_api_client_v2-0.470.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-06-30 16:23:21.763239 stigg_api_client_v2-0.470.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-06-30 16:23:21.721879 stigg_api_client_v2-0.470.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-06-30 16:23:21.711869 stigg_api_client_v2-0.470.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-06-30 16:23:21.781593 stigg_api_client_v2-0.470.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-06-30 16:23:21.701849 stigg_api_client_v2-0.470.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-06-30 16:23:21.737470 stigg_api_client_v2-0.470.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-06-30 16:23:21.752892 stigg_api_client_v2-0.470.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-06-30 16:23:21.510587 stigg_api_client_v2-0.470.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-06-30 16:23:21.501488 stigg_api_client_v2-0.470.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-06-30 16:23:21.547531 stigg_api_client_v2-0.470.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126193 2023-06-30 16:23:21.473438 stigg_api_client_v2-0.470.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-06-30 16:23:21.651368 stigg_api_client_v2-0.470.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-06-30 16:23:21.492844 stigg_api_client_v2-0.470.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-06-30 16:23:21.539696 stigg_api_client_v2-0.470.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-06-30 16:23:21.629696 stigg_api_client_v2-0.470.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-06-30 16:23:21.622568 stigg_api_client_v2-0.470.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-06-30 16:23:21.614976 stigg_api_client_v2-0.470.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-06-30 16:23:23.241030 stigg_api_client_v2-0.470.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-06-30 16:23:21.520747 stigg_api_client_v2-0.470.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-06-30 16:23:21.558933 stigg_api_client_v2-0.470.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-06-30 16:23:21.791442 stigg_api_client_v2-0.470.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.470.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.468.0/README.md` & `stigg_api_client_v2-0.470.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.470.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 
 from .async_base_client import AsyncBaseClient
+from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
     CancelSubscriptionCancelSubscription,
 )
 from .cancel_subscription_updates import CancelSubscriptionUpdates
-from .client import Client
 from .create_subscription import (
     CreateSubscription,
     CreateSubscriptionCreateSubscription,
 )
-from .entitlements_updated import (
-    EntitlementsUpdated,
-    EntitlementsUpdatedEntitlementsUpdated,
-)
 from .enums import (
     AccessDeniedReason,
     AccountStatus,
     AddonSortFields,
     AggregationFunction,
     Alignment,
     ApiKeySortFields,
@@ -602,15 +598,14 @@
 from .report_usage import ReportUsage, ReportUsageCreateUsageMeasurement
 from .update_customer import UpdateCustomer, UpdateCustomerUpdateCustomer
 from .update_subscription import (
     UpdateSubscription,
     UpdateSubscriptionUpdateSubscription,
 )
 from .usage_history import UsageHistory, UsageHistoryUsageHistory
-from .usage_updated import UsageUpdated, UsageUpdatedUsageUpdated
 
 __all__ = [
     "AccessDeniedReason",
     "AccountStatus",
     "AddCompatibleAddonsToPlanInput",
     "AddonCreateInput",
     "AddonFilter",
@@ -626,14 +621,15 @@
     "ApiKeyFilter",
     "ApiKeySort",
     "ApiKeySortFields",
     "ApiKeyType",
     "ArchiveCouponInput",
     "ArchivePlanInput",
     "AsyncBaseClient",
+    "AsyncClient",
     "AttachCustomerPaymentMethodInput",
     "BaseModel",
     "BillableFeatureInput",
     "BillingAnchor",
     "BillingModel",
     "BillingModelFilterComparison",
     "BillingPeriod",
@@ -641,15 +637,14 @@
     "BooleanFieldComparison",
     "CancelSubscription",
     "CancelSubscriptionCancelSubscription",
     "CancelSubscriptionUpdates",
     "ChangeType",
     "CheckoutOptions",
     "ClearCustomerPersistentCacheInput",
-    "Client",
     "ConditionOperation",
     "CouponFilter",
     "CouponFilterCustomerFilter",
     "CouponFragment",
     "CouponFragmentCustomers",
     "CouponFragmentSyncStates",
     "CouponSort",
@@ -767,16 +762,14 @@
     "EntitlementFragmentResetPeriodConfigurationMonthlyResetPeriodConfig",
     "EntitlementFragmentResetPeriodConfigurationWeeklyResetPeriodConfig",
     "EntitlementOptions",
     "EntitlementResetPeriod",
     "EntitlementUsageUpdated",
     "EntitlementUsageUpdatedEntitlement",
     "EntitlementUsageUpdatedUsage",
-    "EntitlementsUpdated",
-    "EntitlementsUpdatedEntitlementsUpdated",
     "EntitlementsUpdatedPayload",
     "EntitlementsUpdatedPayloadEntitlements",
     "EntitySelectionMode",
     "EnvironmentFilter",
     "EnvironmentInput",
     "EnvironmentProvisionStatus",
     "EnvironmentSort",
@@ -1172,17 +1165,15 @@
     "UsageMeasurementCreateInput",
     "UsageMeasurementFilter",
     "UsageMeasurementFilterCustomerFilter",
     "UsageMeasurementFilterFeatureFilter",
     "UsageMeasurementSort",
     "UsageMeasurementSortFields",
     "UsageUpdateBehavior",
-    "UsageUpdated",
     "UsageUpdatedFragment",
-    "UsageUpdatedUsageUpdated",
     "VendorIdentifier",
     "VendorIdentifierFilterComparison",
     "WeeklyAccordingTo",
     "WeeklyResetPeriodConfigInput",
     "WidgetConfigurationUpdateInput",
     "WidgetType",
     "ZuoraCredentialsInput",
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.470.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.470.0/stigg/generated/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.470.0/stigg/generated/cancel_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/client.py` & `stigg_api_client_v2-0.470.0/stigg/generated/async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
-from typing import AsyncIterator
-
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
-from .entitlements_updated import EntitlementsUpdated
 from .estimate_subscription import EstimateSubscription
 from .estimate_subscription_update import EstimateSubscriptionUpdate
 from .get_active_subscriptions import GetActiveSubscriptions
 from .get_coupons import GetCoupons
 from .get_customer_by_id import GetCustomerById
 from .get_customer_portal_by_ref_id import GetCustomerPortalByRefId
 from .get_entitlement import GetEntitlement
@@ -53,22 +50,21 @@
 from .provision_subscription import ProvisionSubscription
 from .report_entitlement_check_requested import ReportEntitlementCheckRequested
 from .report_event import ReportEvent
 from .report_usage import ReportUsage
 from .update_customer import UpdateCustomer
 from .update_subscription import UpdateSubscription
 from .usage_history import UsageHistory
-from .usage_updated import UsageUpdated
 
 
 def gql(q: str) -> str:
     return q
 
 
-class Client(AsyncBaseClient):
+class AsyncClient(AsyncBaseClient):
     async def provision_customer(
         self, input: ProvisionCustomerInput
     ) -> ProvisionCustomer:
         query = gql(
             """
             mutation ProvisionCustomer($input: ProvisionCustomerInput!) {
               provisionCustomer(input: $input) {
@@ -2346,142 +2342,7 @@
             }
             """
         )
         variables: dict[str, object] = {"usageHistoryInput": usage_history_input}
         response = await self.execute(query=query, variables=variables)
         data = self.get_data(response)
         return UsageHistory.parse_obj(data)
-
-    async def entitlements_updated(self) -> AsyncIterator[EntitlementsUpdated]:
-        query = gql(
-            """
-            subscription EntitlementsUpdated {
-              entitlementsUpdated {
-                ...EntitlementsUpdatedPayload
-              }
-            }
-
-            fragment EntitlementFragment on Entitlement {
-              isGranted
-              accessDeniedReason
-              customerId
-              resourceId
-              usageLimit
-              hasUnlimitedUsage
-              currentUsage
-              requestedUsage
-              entitlementUpdatedAt
-              usageUpdatedAt
-              nextResetDate
-              resetPeriod
-              resetPeriodConfiguration {
-                ...ResetPeriodConfigurationFragment
-              }
-              feature {
-                ...FeatureFragment
-              }
-            }
-
-            fragment EntitlementsUpdatedPayload on EntitlementsUpdated {
-              customerId
-              resourceId
-              entitlements {
-                ...EntitlementFragment
-              }
-            }
-
-            fragment FeatureFragment on EntitlementFeature {
-              featureType
-              meterType
-              featureUnits
-              featureUnitsPlural
-              description
-              displayName
-              refId
-            }
-
-            fragment ResetPeriodConfigurationFragment on ResetPeriodConfiguration {
-              __typename
-              ... on MonthlyResetPeriodConfig {
-                monthlyAccordingTo
-              }
-              ... on WeeklyResetPeriodConfig {
-                weeklyAccordingTo
-              }
-            }
-            """
-        )
-        variables: dict[str, object] = {}
-        async for data in self.execute_ws(query=query, variables=variables):
-            yield EntitlementsUpdated.parse_obj(data)
-
-    async def usage_updated(self) -> AsyncIterator[UsageUpdated]:
-        query = gql(
-            """
-            subscription UsageUpdated {
-              usageUpdated {
-                ...EntitlementUsageUpdated
-              }
-            }
-
-            fragment EntitlementFragment on Entitlement {
-              isGranted
-              accessDeniedReason
-              customerId
-              resourceId
-              usageLimit
-              hasUnlimitedUsage
-              currentUsage
-              requestedUsage
-              entitlementUpdatedAt
-              usageUpdatedAt
-              nextResetDate
-              resetPeriod
-              resetPeriodConfiguration {
-                ...ResetPeriodConfigurationFragment
-              }
-              feature {
-                ...FeatureFragment
-              }
-            }
-
-            fragment EntitlementUsageUpdated on UsageUpdated {
-              usage {
-                ...UsageUpdatedFragment
-              }
-              entitlement {
-                ...EntitlementFragment
-              }
-            }
-
-            fragment FeatureFragment on EntitlementFeature {
-              featureType
-              meterType
-              featureUnits
-              featureUnitsPlural
-              description
-              displayName
-              refId
-            }
-
-            fragment ResetPeriodConfigurationFragment on ResetPeriodConfiguration {
-              __typename
-              ... on MonthlyResetPeriodConfig {
-                monthlyAccordingTo
-              }
-              ... on WeeklyResetPeriodConfig {
-                weeklyAccordingTo
-              }
-            }
-
-            fragment UsageUpdatedFragment on UsageMeasurementUpdated {
-              customerId
-              resourceId
-              featureId
-              currentUsage
-              nextResetDate
-            }
-            """
-        )
-        variables: dict[str, object] = {}
-        async for data in self.execute_ws(query=query, variables=variables):
-            yield UsageUpdated.parse_obj(data)
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.470.0/stigg/generated/create_subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.470.0/stigg/generated/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerNotFound = "CustomerNotFound"
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.470.0/stigg/generated/estimate_subscription_update.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.470.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.470.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -124,25 +124,14 @@
     status: SyncStatus
 
 
 class CouponFragmentCustomers(BaseModel):
     id: str
 
 
-class SlimCustomerFragment(BaseModel):
-    id: str
-    name: Optional[str]
-    email: Optional[str]
-    created_at: Optional[Any] = Field(alias="createdAt")
-    updated_at: Any = Field(alias="updatedAt")
-    ref_id: str = Field(alias="refId")
-    billing_id: Optional[str] = Field(alias="billingId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class PromotionalEntitlementFragment(BaseModel):
     status: PromotionalEntitlementStatus
     usage_limit: Optional[float] = Field(alias="usageLimit")
     feature_id: str = Field(alias="featureId")
     has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
     reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
     end_date: Optional[Any] = Field(alias="endDate")
@@ -157,14 +146,25 @@
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     ref_id: str = Field(alias="refId")
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
 
 
+class SlimCustomerFragment(BaseModel):
+    id: str
+    name: Optional[str]
+    email: Optional[str]
+    created_at: Optional[Any] = Field(alias="createdAt")
+    updated_at: Any = Field(alias="updatedAt")
+    ref_id: str = Field(alias="refId")
+    billing_id: Optional[str] = Field(alias="billingId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class CustomerFragment(SlimCustomerFragment):
     has_payment_method: bool = Field(alias="hasPaymentMethod")
     has_active_subscription: bool = Field(alias="hasActiveSubscription")
     default_payment_expiration_month: Optional[int] = Field(
         alias="defaultPaymentExpirationMonth"
     )
     default_payment_expiration_year: Optional[int] = Field(
@@ -328,19 +328,21 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
-class CustomerPortalSubscriptionAddon(BaseModel):
-    addon_id: str = Field(alias="addonId")
-    description: Optional[str]
+class CustomerPortalPromotionalEntitlement(BaseModel):
     display_name: str = Field(alias="displayName")
-    quantity: int
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
 
 
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
@@ -386,14 +388,21 @@
     BaseModel
 ):
     typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
     new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
     feature_id: Optional[str] = Field(alias="featureId")
 
 
+class CustomerPortalSubscriptionAddon(BaseModel):
+    addon_id: str = Field(alias="addonId")
+    description: Optional[str]
+    display_name: str = Field(alias="displayName")
+    quantity: int
+
+
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
     trial_remaining_days: Optional[int] = Field(alias="trialRemainingDays")
     billing_period_range: Optional[
@@ -466,23 +475,14 @@
     pass
 
 
 class CustomerResourceFragment(BaseModel):
     resource_id: str = Field(alias="resourceId")
 
 
-class CustomerPortalPromotionalEntitlement(BaseModel):
-    display_name: str = Field(alias="displayName")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    period: PromotionalEntitlementPeriod
-    start_date: Any = Field(alias="startDate")
-    end_date: Optional[Any] = Field(alias="endDate")
-
-
 class CustomerPortalFragment(BaseModel):
     subscriptions: List["CustomerPortalFragmentSubscriptions"]
     entitlements: List["CustomerPortalFragmentEntitlements"]
     promotional_entitlements: List[
         "CustomerPortalFragmentPromotionalEntitlements"
     ] = Field(alias="promotionalEntitlements")
     billing_information: "CustomerPortalFragmentBillingInformation" = Field(
@@ -517,27 +517,63 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
+class SubscriptionScheduledUpdateData(BaseModel):
+    subscription_schedule_type: SubscriptionScheduleType = Field(
+        alias="subscriptionScheduleType"
+    )
+    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
+    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
+    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
+        alias="targetPackage"
+    )
+    schedule_variables: Optional[
+        Annotated[
+            Union[
+                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
+                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
+            ],
+            Field(discriminator="typename__"),
+        ]
+    ] = Field(alias="scheduleVariables")
 
 
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
+class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
 
 
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
+class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
+    BaseModel
+):
+    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
+    BaseModel
+):
+    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
+    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+
+
+class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
+    BaseModel
+):
+    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
+    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
+    feature_id: Optional[str] = Field(alias="featureId")
 
 
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -604,63 +640,27 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
-class SubscriptionScheduledUpdateData(BaseModel):
-    subscription_schedule_type: SubscriptionScheduleType = Field(
-        alias="subscriptionScheduleType"
-    )
-    schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
-    scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
-    target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
-        alias="targetPackage"
-    )
-    schedule_variables: Optional[
-        Annotated[
-            Union[
-                "SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables",
-                "SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables",
-            ],
-            Field(discriminator="typename__"),
-        ]
-    ] = Field(alias="scheduleVariables")
-
-
-class SubscriptionScheduledUpdateDataTargetPackage(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-
-
-class SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables(
-    BaseModel
-):
-    typename__: Literal["BillingPeriodChangeVariables"] = Field(alias="__typename")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables(
-    BaseModel
-):
-    typename__: Literal["DowngradeChangeVariables"] = Field(alias="__typename")
-    addon_ref_ids: Optional[str] = Field(alias="addonRefIds")
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    downgrade_plan_ref_id: str = Field(alias="downgradePlanRefId")
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
 
 
-class SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables(
-    BaseModel
-):
-    typename__: Literal["UnitAmountChangeVariables"] = Field(alias="__typename")
-    new_unit_amount: Optional[float] = Field(alias="newUnitAmount")
-    feature_id: Optional[str] = Field(alias="featureId")
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
 
 
 class SubscriptionFragment(BaseModel):
     id: str
     start_date: Any = Field(alias="startDate")
     end_date: Optional[Any] = Field(alias="endDate")
     trial_end_date: Optional[Any] = Field(alias="trialEndDate")
@@ -1293,17 +1293,17 @@
 PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
-SlimCustomerFragment.update_forward_refs()
 PromotionalEntitlementFragment.update_forward_refs()
 PromotionalEntitlementFragmentFeature.update_forward_refs()
+SlimCustomerFragment.update_forward_refs()
 CustomerFragment.update_forward_refs()
 CustomerFragmentTrialedPlans.update_forward_refs()
 CustomerFragmentExperimentInfo.update_forward_refs()
 CustomerFragmentCoupon.update_forward_refs()
 CustomerFragmentEligibleForTrial.update_forward_refs()
 CustomerFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalBillingInformation.update_forward_refs()
@@ -1317,59 +1317,59 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
-CustomerPortalSubscriptionAddon.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+CustomerPortalSubscriptionAddon.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricing.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentPricingFeature.update_forward_refs()
 CustomerPortalSubscriptionFragmentBillingPeriodRange.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPrice.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceSubTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentTotalPriceAddonsTotal.update_forward_refs()
 CustomerPortalSubscriptionFragmentAddons.update_forward_refs()
 CustomerPortalSubscriptionFragmentScheduledUpdates.update_forward_refs()
 CustomerResourceFragment.update_forward_refs()
-CustomerPortalPromotionalEntitlement.update_forward_refs()
 CustomerPortalFragment.update_forward_refs()
 CustomerPortalFragmentSubscriptions.update_forward_refs()
 CustomerPortalFragmentEntitlements.update_forward_refs()
 CustomerPortalFragmentPromotionalEntitlements.update_forward_refs()
 CustomerPortalFragmentBillingInformation.update_forward_refs()
 CustomerPortalFragmentConfiguration.update_forward_refs()
 CustomerPortalFragmentResource.update_forward_refs()
-TotalPriceFragment.update_forward_refs()
-TotalPriceFragmentSubTotal.update_forward_refs()
-TotalPriceFragmentTotal.update_forward_refs()
+SubscriptionScheduledUpdateData.update_forward_refs()
+SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
+SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 ProductFragment.update_forward_refs()
 ProductFragmentProductSettings.update_forward_refs()
 ProductFragmentProductSettingsDowngradePlan.update_forward_refs()
 PlanFragment.update_forward_refs()
 PlanFragmentProduct.update_forward_refs()
 PlanFragmentBasePlan.update_forward_refs()
 PlanFragmentEntitlements.update_forward_refs()
 PlanFragmentInheritedEntitlements.update_forward_refs()
 PlanFragmentCompatibleAddons.update_forward_refs()
 PlanFragmentPrices.update_forward_refs()
 PlanFragmentDefaultTrialConfig.update_forward_refs()
-SubscriptionScheduledUpdateData.update_forward_refs()
-SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
-SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
 SubscriptionFragmentExperimentInfo.update_forward_refs()
 SubscriptionFragmentPrices.update_forward_refs()
 SubscriptionFragmentPricesPrice.update_forward_refs()
 SubscriptionFragmentTotalPrice.update_forward_refs()
 SubscriptionFragmentPlan.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_customer_by_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_mock_paywall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_products.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.470.0/stigg/generated/get_sdk_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.470.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.470.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.470.0/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.470.0/stigg/generated/provision_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.468.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.470.0/stigg/generated/update_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-06-26 16:36
+# Generated by ariadne-codegen on 2023-06-30 19:23
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.468.0/PKG-INFO` & `stigg_api_client_v2-0.470.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.468.0
+Version: 0.470.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

