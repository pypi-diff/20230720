# Comparing `tmp/stigg_api_client_v2-0.493.0.tar.gz` & `tmp/stigg_api_client_v2-0.496.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stigg_api_client_v2-0.493.0.tar", max compression
+gzip compressed data, was "stigg_api_client_v2-0.496.0.tar", max compression
```

## Comparing `stigg_api_client_v2-0.493.0.tar` & `stigg_api_client_v2-0.496.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1644 2023-07-19 06:41:41.849078 stigg_api_client_v2-0.493.0/README.md
--rw-r--r--   0        0        0      432 2023-07-19 06:42:28.825683 stigg_api_client_v2-0.493.0/pyproject.toml
--rw-r--r--   0        0        0       62 2023-07-19 06:41:41.849078 stigg_api_client_v2-0.493.0/stigg/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-19 06:41:41.849078 stigg_api_client_v2-0.493.0/stigg/client.py
--rw-r--r--   0        0        0    40178 2023-07-19 06:42:27.145663 stigg_api_client_v2-0.493.0/stigg/generated/__init__.py
--rw-r--r--   0        0        0      460 2023-07-19 06:42:25.781647 stigg_api_client_v2-0.493.0/stigg/generated/archive_customer.py
--rw-r--r--   0        0        0     7303 2023-07-19 06:42:26.769659 stigg_api_client_v2-0.493.0/stigg/generated/async_base_client.py
--rw-r--r--   0        0        0    68230 2023-07-19 06:42:26.985661 stigg_api_client_v2-0.493.0/stigg/generated/async_client.py
--rw-r--r--   0        0        0     2731 2023-07-19 06:42:21.801594 stigg_api_client_v2-0.493.0/stigg/generated/base_client.py
--rw-r--r--   0        0        0     1951 2023-07-19 06:42:26.769659 stigg_api_client_v2-0.493.0/stigg/generated/base_model.py
--rw-r--r--   0        0        0      527 2023-07-19 06:42:25.725646 stigg_api_client_v2-0.493.0/stigg/generated/cancel_subscription.py
--rw-r--r--   0        0        0      296 2023-07-19 06:42:25.745646 stigg_api_client_v2-0.493.0/stigg/generated/cancel_subscription_updates.py
--rw-r--r--   0        0        0    67803 2023-07-19 06:42:22.041597 stigg_api_client_v2-0.493.0/stigg/generated/client.py
--rw-r--r--   0        0        0      527 2023-07-19 06:42:25.769647 stigg_api_client_v2-0.493.0/stigg/generated/create_subscription.py
--rw-r--r--   0        0        0    24102 2023-07-19 06:42:23.533617 stigg_api_client_v2-0.493.0/stigg/generated/enums.py
--rw-r--r--   0        0        0      553 2023-07-19 06:42:25.733646 stigg_api_client_v2-0.493.0/stigg/generated/estimate_subscription.py
--rw-r--r--   0        0        0      614 2023-07-19 06:42:25.737646 stigg_api_client_v2-0.493.0/stigg/generated/estimate_subscription_update.py
--rw-r--r--   0        0        0     2366 2023-07-19 06:42:26.769659 stigg_api_client_v2-0.493.0/stigg/generated/exceptions.py
--rw-r--r--   0        0        0    56292 2023-07-19 06:42:26.769659 stigg_api_client_v2-0.493.0/stigg/generated/fragments.py
--rw-r--r--   0        0        0      591 2023-07-19 06:42:25.797647 stigg_api_client_v2-0.493.0/stigg/generated/get_active_subscriptions.py
--rw-r--r--   0        0        0      634 2023-07-19 06:42:25.805647 stigg_api_client_v2-0.493.0/stigg/generated/get_coupons.py
--rw-r--r--   0        0        0      572 2023-07-19 06:42:25.789647 stigg_api_client_v2-0.493.0/stigg/generated/get_customer_by_id.py
--rw-r--r--   0        0        0      533 2023-07-19 06:42:25.845647 stigg_api_client_v2-0.493.0/stigg/generated/get_customer_portal_by_ref_id.py
--rw-r--r--   0        0        0      390 2023-07-19 06:42:25.821647 stigg_api_client_v2-0.493.0/stigg/generated/get_entitlement.py
--rw-r--r--   0        0        0      430 2023-07-19 06:42:25.813647 stigg_api_client_v2-0.493.0/stigg/generated/get_entitlements.py
--rw-r--r--   0        0        0      893 2023-07-19 06:42:25.857648 stigg_api_client_v2-0.493.0/stigg/generated/get_mock_paywall.py
--rw-r--r--   0        0        0      346 2023-07-19 06:42:25.809647 stigg_api_client_v2-0.493.0/stigg/generated/get_paywall.py
--rw-r--r--   0        0        0      657 2023-07-19 06:42:25.829647 stigg_api_client_v2-0.493.0/stigg/generated/get_products.py
--rw-r--r--   0        0        0      650 2023-07-19 06:42:25.841647 stigg_api_client_v2-0.493.0/stigg/generated/get_sdk_configuration.py
--rw-r--r--   0        0        0      465 2023-07-19 06:42:25.689645 stigg_api_client_v2-0.493.0/stigg/generated/import_customer.py
--rw-r--r--   0        0        0      332 2023-07-19 06:42:25.681645 stigg_api_client_v2-0.493.0/stigg/generated/import_customer_bulk.py
--rw-r--r--   0        0        0      350 2023-07-19 06:42:25.713646 stigg_api_client_v2-0.493.0/stigg/generated/import_subscriptions_bulk.py
--rw-r--r--   0        0        0   126537 2023-07-19 06:42:25.665645 stigg_api_client_v2-0.493.0/stigg/generated/input_types.py
--rw-r--r--   0        0        0      604 2023-07-19 06:42:25.777646 stigg_api_client_v2-0.493.0/stigg/generated/migrate_subscription_to_latest.py
--rw-r--r--   0        0        0     1161 2023-07-19 06:42:25.677645 stigg_api_client_v2-0.493.0/stigg/generated/provision_customer.py
--rw-r--r--   0        0        0      971 2023-07-19 06:42:25.709646 stigg_api_client_v2-0.493.0/stigg/generated/provision_subscription.py
--rw-r--r--   0        0        0      359 2023-07-19 06:42:25.761646 stigg_api_client_v2-0.493.0/stigg/generated/report_entitlement_check_requested.py
--rw-r--r--   0        0        0      301 2023-07-19 06:42:25.757646 stigg_api_client_v2-0.493.0/stigg/generated/report_event.py
--rw-r--r--   0        0        0      637 2023-07-19 06:42:25.753646 stigg_api_client_v2-0.493.0/stigg/generated/report_usage.py
--rw-r--r--   0        0        0      220 2023-07-19 06:42:26.773659 stigg_api_client_v2-0.493.0/stigg/generated/scalars.py
--rw-r--r--   0        0        0      465 2023-07-19 06:42:25.693645 stigg_api_client_v2-0.493.0/stigg/generated/update_customer.py
--rw-r--r--   0        0        0      527 2023-07-19 06:42:25.721646 stigg_api_client_v2-0.493.0/stigg/generated/update_subscription.py
--rw-r--r--   0        0        0      445 2023-07-19 06:42:25.861648 stigg_api_client_v2-0.493.0/stigg/generated/usage_history.py
--rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.493.0/PKG-INFO
+-rw-r--r--   0        0        0     1644 2023-07-20 15:44:04.911350 stigg_api_client_v2-0.496.0/README.md
+-rw-r--r--   0        0        0      432 2023-07-20 15:44:49.271891 stigg_api_client_v2-0.496.0/pyproject.toml
+-rw-r--r--   0        0        0       62 2023-07-20 15:44:04.915350 stigg_api_client_v2-0.496.0/stigg/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-20 15:44:04.915350 stigg_api_client_v2-0.496.0/stigg/client.py
+-rw-r--r--   0        0        0    40178 2023-07-20 15:44:47.591872 stigg_api_client_v2-0.496.0/stigg/generated/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-20 15:44:46.343873 stigg_api_client_v2-0.496.0/stigg/generated/archive_customer.py
+-rw-r--r--   0        0        0     7303 2023-07-20 15:44:47.211871 stigg_api_client_v2-0.496.0/stigg/generated/async_base_client.py
+-rw-r--r--   0        0        0    68230 2023-07-20 15:44:47.431871 stigg_api_client_v2-0.496.0/stigg/generated/async_client.py
+-rw-r--r--   0        0        0     2731 2023-07-20 15:44:42.283854 stigg_api_client_v2-0.496.0/stigg/generated/base_client.py
+-rw-r--r--   0        0        0     1951 2023-07-20 15:44:47.211871 stigg_api_client_v2-0.496.0/stigg/generated/base_model.py
+-rw-r--r--   0        0        0      527 2023-07-20 15:44:46.291874 stigg_api_client_v2-0.496.0/stigg/generated/cancel_subscription.py
+-rw-r--r--   0        0        0      296 2023-07-20 15:44:46.307873 stigg_api_client_v2-0.496.0/stigg/generated/cancel_subscription_updates.py
+-rw-r--r--   0        0        0    67803 2023-07-20 15:44:42.503857 stigg_api_client_v2-0.496.0/stigg/generated/client.py
+-rw-r--r--   0        0        0      527 2023-07-20 15:44:46.331873 stigg_api_client_v2-0.496.0/stigg/generated/create_subscription.py
+-rw-r--r--   0        0        0    24160 2023-07-20 15:44:44.007876 stigg_api_client_v2-0.496.0/stigg/generated/enums.py
+-rw-r--r--   0        0        0      553 2023-07-20 15:44:46.295873 stigg_api_client_v2-0.496.0/stigg/generated/estimate_subscription.py
+-rw-r--r--   0        0        0      614 2023-07-20 15:44:46.303873 stigg_api_client_v2-0.496.0/stigg/generated/estimate_subscription_update.py
+-rw-r--r--   0        0        0     2366 2023-07-20 15:44:47.211871 stigg_api_client_v2-0.496.0/stigg/generated/exceptions.py
+-rw-r--r--   0        0        0    56292 2023-07-20 15:44:47.207871 stigg_api_client_v2-0.496.0/stigg/generated/fragments.py
+-rw-r--r--   0        0        0      591 2023-07-20 15:44:46.359873 stigg_api_client_v2-0.496.0/stigg/generated/get_active_subscriptions.py
+-rw-r--r--   0        0        0      634 2023-07-20 15:44:46.367873 stigg_api_client_v2-0.496.0/stigg/generated/get_coupons.py
+-rw-r--r--   0        0        0      572 2023-07-20 15:44:46.351873 stigg_api_client_v2-0.496.0/stigg/generated/get_customer_by_id.py
+-rw-r--r--   0        0        0      533 2023-07-20 15:44:46.403873 stigg_api_client_v2-0.496.0/stigg/generated/get_customer_portal_by_ref_id.py
+-rw-r--r--   0        0        0      390 2023-07-20 15:44:46.383873 stigg_api_client_v2-0.496.0/stigg/generated/get_entitlement.py
+-rw-r--r--   0        0        0      430 2023-07-20 15:44:46.375873 stigg_api_client_v2-0.496.0/stigg/generated/get_entitlements.py
+-rw-r--r--   0        0        0      893 2023-07-20 15:44:46.415873 stigg_api_client_v2-0.496.0/stigg/generated/get_mock_paywall.py
+-rw-r--r--   0        0        0      346 2023-07-20 15:44:46.371873 stigg_api_client_v2-0.496.0/stigg/generated/get_paywall.py
+-rw-r--r--   0        0        0      657 2023-07-20 15:44:46.387873 stigg_api_client_v2-0.496.0/stigg/generated/get_products.py
+-rw-r--r--   0        0        0      650 2023-07-20 15:44:46.399873 stigg_api_client_v2-0.496.0/stigg/generated/get_sdk_configuration.py
+-rw-r--r--   0        0        0      465 2023-07-20 15:44:46.259873 stigg_api_client_v2-0.496.0/stigg/generated/import_customer.py
+-rw-r--r--   0        0        0      332 2023-07-20 15:44:46.251874 stigg_api_client_v2-0.496.0/stigg/generated/import_customer_bulk.py
+-rw-r--r--   0        0        0      350 2023-07-20 15:44:46.279873 stigg_api_client_v2-0.496.0/stigg/generated/import_subscriptions_bulk.py
+-rw-r--r--   0        0        0   126537 2023-07-20 15:44:46.235874 stigg_api_client_v2-0.496.0/stigg/generated/input_types.py
+-rw-r--r--   0        0        0      604 2023-07-20 15:44:46.339873 stigg_api_client_v2-0.496.0/stigg/generated/migrate_subscription_to_latest.py
+-rw-r--r--   0        0        0     1161 2023-07-20 15:44:46.247874 stigg_api_client_v2-0.496.0/stigg/generated/provision_customer.py
+-rw-r--r--   0        0        0      971 2023-07-20 15:44:46.271874 stigg_api_client_v2-0.496.0/stigg/generated/provision_subscription.py
+-rw-r--r--   0        0        0      359 2023-07-20 15:44:46.327873 stigg_api_client_v2-0.496.0/stigg/generated/report_entitlement_check_requested.py
+-rw-r--r--   0        0        0      301 2023-07-20 15:44:46.319873 stigg_api_client_v2-0.496.0/stigg/generated/report_event.py
+-rw-r--r--   0        0        0      637 2023-07-20 15:44:46.315873 stigg_api_client_v2-0.496.0/stigg/generated/report_usage.py
+-rw-r--r--   0        0        0      220 2023-07-20 15:44:47.215871 stigg_api_client_v2-0.496.0/stigg/generated/scalars.py
+-rw-r--r--   0        0        0      465 2023-07-20 15:44:46.263874 stigg_api_client_v2-0.496.0/stigg/generated/update_customer.py
+-rw-r--r--   0        0        0      527 2023-07-20 15:44:46.283873 stigg_api_client_v2-0.496.0/stigg/generated/update_subscription.py
+-rw-r--r--   0        0        0      445 2023-07-20 15:44:46.419873 stigg_api_client_v2-0.496.0/stigg/generated/usage_history.py
+-rw-r--r--   0        0        0     2034 1970-01-01 00:00:00.000000 stigg_api_client_v2-0.496.0/PKG-INFO
```

### Comparing `stigg_api_client_v2-0.493.0/README.md` & `stigg_api_client_v2-0.496.0/README.md`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.493.0/stigg/client.py` & `stigg_api_client_v2-0.496.0/stigg/client.py`

 * *Files identical despite different names*

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/__init__.py` & `stigg_api_client_v2-0.496.0/stigg/generated/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 
 from .archive_customer import ArchiveCustomer, ArchiveCustomerArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .async_client import AsyncClient
 from .base_model import BaseModel
 from .cancel_subscription import (
     CancelSubscription,
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/async_base_client.py` & `stigg_api_client_v2-0.496.0/stigg/generated/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 
 import enum
 import json
 from typing import Any, AsyncIterator, Dict, Optional, TypeVar, cast
 from uuid import uuid4
 
 import httpx
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/async_client.py` & `stigg_api_client_v2-0.496.0/stigg/generated/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .async_base_client import AsyncBaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/base_client.py` & `stigg_api_client_v2-0.496.0/stigg/generated/base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 
 import json
 from typing import Any, Dict, Optional, TypeVar, cast
 
 import httpx
 from pydantic import BaseModel
 from pydantic.json import pydantic_encoder
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/base_model.py` & `stigg_api_client_v2-0.496.0/stigg/generated/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 
 from typing import Any, Dict, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel as PydanticBaseModel
 from pydantic.class_validators import validator
 from pydantic.fields import ModelField
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/cancel_subscription.py` & `stigg_api_client_v2-0.496.0/stigg/generated/cancel_subscription.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/client.py` & `stigg_api_client_v2-0.496.0/stigg/generated/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from .archive_customer import ArchiveCustomer
 from .base_client import BaseClient
 from .cancel_subscription import CancelSubscription
 from .cancel_subscription_updates import CancelSubscriptionUpdates
 from .create_subscription import CreateSubscription
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/create_subscription.py` & `stigg_api_client_v2-0.496.0/stigg/generated/create_subscription.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/enums.py` & `stigg_api_client_v2-0.496.0/stigg/generated/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from enum import Enum
 
 
 class AccessDeniedReason(str, Enum):
     CustomerIsArchived = "CustomerIsArchived"
@@ -706,14 +706,15 @@
     NULLS_FIRST = "NULLS_FIRST"
     NULLS_LAST = "NULLS_LAST"
 
 
 class SourceType(str, Enum):
     JS_CLIENT_SDK = "JS_CLIENT_SDK"
     NODE_SERVER_SDK = "NODE_SERVER_SDK"
+    PERSISTENT_CACHE_SERVICE = "PERSISTENT_CACHE_SERVICE"
 
 
 class SubscriptionAddonSortFields(str, Enum):
     createdAt = "createdAt"
     id = "id"
     quantity = "quantity"
     updatedAt = "updatedAt"
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/estimate_subscription.py` & `stigg_api_client_v2-0.496.0/stigg/generated/estimate_subscription.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/estimate_subscription_update.py` & `stigg_api_client_v2-0.496.0/stigg/generated/estimate_subscription_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SubscriptionPreviewFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/exceptions.py` & `stigg_api_client_v2-0.496.0/stigg/generated/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 
 class GraphQLClientError(Exception):
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/fragments.py` & `stigg_api_client_v2-0.496.0/stigg/generated/fragments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import Annotated, Any, List, Literal, Optional, Union
 
 from pydantic import Field
 
 from .base_model import BaseModel
@@ -32,14 +32,36 @@
     VendorIdentifier,
     WeeklyAccordingTo,
     WidgetType,
     experimentGroupType,
 )
 
 
+class PackageEntitlementFragment(BaseModel):
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    feature_id: str = Field(alias="featureId")
+    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
+    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
+    is_custom: Optional[bool] = Field(alias="isCustom")
+    display_name_override: Optional[str] = Field(alias="displayNameOverride")
+    feature: "PackageEntitlementFragmentFeature"
+
+
+class PackageEntitlementFragmentFeature(BaseModel):
+    feature_type: FeatureType = Field(alias="featureType")
+    meter_type: Optional[MeterType] = Field(alias="meterType")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+    display_name: str = Field(alias="displayName")
+    description: Optional[str]
+    ref_id: str = Field(alias="refId")
+    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
+
+
 class PriceFragment(BaseModel):
     billing_model: BillingModel = Field(alias="billingModel")
     billing_period: BillingPeriod = Field(alias="billingPeriod")
     billing_id: Optional[str] = Field(alias="billingId")
     min_unit_quantity: Optional[float] = Field(alias="minUnitQuantity")
     max_unit_quantity: Optional[float] = Field(alias="maxUnitQuantity")
     billing_country_code: Optional[str] = Field(alias="billingCountryCode")
@@ -56,36 +78,14 @@
     ref_id: str = Field(alias="refId")
     feature_units: Optional[str] = Field(alias="featureUnits")
     feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
 
 
-class PackageEntitlementFragment(BaseModel):
-    usage_limit: Optional[float] = Field(alias="usageLimit")
-    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
-    feature_id: str = Field(alias="featureId")
-    reset_period: Optional[EntitlementResetPeriod] = Field(alias="resetPeriod")
-    hidden_from_widgets: Optional[List[WidgetType]] = Field(alias="hiddenFromWidgets")
-    is_custom: Optional[bool] = Field(alias="isCustom")
-    display_name_override: Optional[str] = Field(alias="displayNameOverride")
-    feature: "PackageEntitlementFragmentFeature"
-
-
-class PackageEntitlementFragmentFeature(BaseModel):
-    feature_type: FeatureType = Field(alias="featureType")
-    meter_type: Optional[MeterType] = Field(alias="meterType")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-    display_name: str = Field(alias="displayName")
-    description: Optional[str]
-    ref_id: str = Field(alias="refId")
-    additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
-
-
 class AddonFragment(BaseModel):
     id: str
     ref_id: str = Field(alias="refId")
     billing_id: Optional[str] = Field(alias="billingId")
     display_name: str = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
@@ -329,14 +329,47 @@
     weekly_according_to: Optional[WeeklyAccordingTo] = Field(alias="weeklyAccordingTo")
 
 
 class CustomerPortalEntitlementFeature(FeatureFragment):
     pass
 
 
+class CustomerPortalPromotionalEntitlement(BaseModel):
+    display_name: str = Field(alias="displayName")
+    has_unlimited_usage: Optional[bool] = Field(alias="hasUnlimitedUsage")
+    usage_limit: Optional[float] = Field(alias="usageLimit")
+    period: PromotionalEntitlementPeriod
+    start_date: Any = Field(alias="startDate")
+    end_date: Optional[Any] = Field(alias="endDate")
+
+
+class CustomerResourceFragment(BaseModel):
+    resource_id: str = Field(alias="resourceId")
+
+
+class CustomerPortalSubscriptionPriceFragment(BaseModel):
+    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
+    billing_model: Optional[BillingModel] = Field(alias="billingModel")
+    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
+    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
+
+
+class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
+    id: str
+    ref_id: str = Field(alias="refId")
+    display_name: str = Field(alias="displayName")
+    feature_units: Optional[str] = Field(alias="featureUnits")
+    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
+
+
 class CustomerPortalSubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional[
@@ -388,34 +421,14 @@
 class CustomerPortalSubscriptionAddon(BaseModel):
     addon_id: str = Field(alias="addonId")
     description: Optional[str]
     display_name: str = Field(alias="displayName")
     quantity: int
 
 
-class CustomerPortalSubscriptionPriceFragment(BaseModel):
-    billing_period: Optional[BillingPeriod] = Field(alias="billingPeriod")
-    billing_model: Optional[BillingModel] = Field(alias="billingModel")
-    price: Optional["CustomerPortalSubscriptionPriceFragmentPrice"]
-    feature: Optional["CustomerPortalSubscriptionPriceFragmentFeature"]
-
-
-class CustomerPortalSubscriptionPriceFragmentPrice(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class CustomerPortalSubscriptionPriceFragmentFeature(BaseModel):
-    id: str
-    ref_id: str = Field(alias="refId")
-    display_name: str = Field(alias="displayName")
-    feature_units: Optional[str] = Field(alias="featureUnits")
-    feature_units_plural: Optional[str] = Field(alias="featureUnitsPlural")
-
-
 class CustomerPortalSubscriptionFragment(BaseModel):
     subscription_id: str = Field(alias="subscriptionId")
     plan_name: str = Field(alias="planName")
     pricing_type: PricingType = Field(alias="pricingType")
     prices: List["CustomerPortalSubscriptionFragmentPrices"]
     pricing: "CustomerPortalSubscriptionFragmentPricing"
     status: SubscriptionStatus
@@ -493,27 +506,14 @@
 
 class CustomerPortalSubscriptionFragmentScheduledUpdates(
     CustomerPortalSubscriptionScheduledUpdateData
 ):
     pass
 
 
-class CustomerResourceFragment(BaseModel):
-    resource_id: str = Field(alias="resourceId")
-
-
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
@@ -548,29 +548,14 @@
     pass
 
 
 class CustomerPortalFragmentResource(CustomerResourceFragment):
     pass
 
 
-class TotalPriceFragment(BaseModel):
-    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
-    total: "TotalPriceFragmentTotal"
-
-
-class TotalPriceFragmentSubTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
-class TotalPriceFragmentTotal(BaseModel):
-    amount: float
-    currency: Currency
-
-
 class ProductFragment(BaseModel):
     ref_id: str = Field(alias="refId")
     display_name: Optional[str] = Field(alias="displayName")
     description: Optional[str]
     additional_meta_data: Optional[Any] = Field(alias="additionalMetaData")
     product_settings: "ProductFragmentProductSettings" = Field(alias="productSettings")
 
@@ -635,14 +620,29 @@
 
 
 class PlanFragmentDefaultTrialConfig(BaseModel):
     duration: float
     units: TrialPeriodUnits
 
 
+class TotalPriceFragment(BaseModel):
+    sub_total: "TotalPriceFragmentSubTotal" = Field(alias="subTotal")
+    total: "TotalPriceFragmentTotal"
+
+
+class TotalPriceFragmentSubTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
+class TotalPriceFragmentTotal(BaseModel):
+    amount: float
+    currency: Currency
+
+
 class SubscriptionScheduledUpdateData(BaseModel):
     subscription_schedule_type: SubscriptionScheduleType = Field(
         alias="subscriptionScheduleType"
     )
     schedule_status: SubscriptionScheduleStatus = Field(alias="scheduleStatus")
     scheduled_execution_time: Any = Field(alias="scheduledExecutionTime")
     target_package: Optional["SubscriptionScheduledUpdateDataTargetPackage"] = Field(
@@ -1341,19 +1341,19 @@
 
 class UsageHistoryFragmentUsageMeasurements(BaseModel):
     date: Any
     value: float
     is_reset_point: Optional[bool] = Field(alias="isResetPoint")
 
 
+PackageEntitlementFragment.update_forward_refs()
+PackageEntitlementFragmentFeature.update_forward_refs()
 PriceFragment.update_forward_refs()
 PriceFragmentPrice.update_forward_refs()
 PriceFragmentFeature.update_forward_refs()
-PackageEntitlementFragment.update_forward_refs()
-PackageEntitlementFragmentFeature.update_forward_refs()
 AddonFragment.update_forward_refs()
 AddonFragmentEntitlements.update_forward_refs()
 AddonFragmentPrices.update_forward_refs()
 CouponFragment.update_forward_refs()
 CouponFragmentSyncStates.update_forward_refs()
 CouponFragmentCustomers.update_forward_refs()
 SlimCustomerFragment.update_forward_refs()
@@ -1376,58 +1376,58 @@
 CustomerPortalConfigurationFragmentPalette.update_forward_refs()
 CustomerPortalConfigurationFragmentTypography.update_forward_refs()
 FeatureFragment.update_forward_refs()
 CustomerPortalEntitlement.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationMonthlyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementResetPeriodConfigurationWeeklyResetPeriodConfig.update_forward_refs()
 CustomerPortalEntitlementFeature.update_forward_refs()
+CustomerPortalPromotionalEntitlement.update_forward_refs()
+CustomerResourceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragment.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
+CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateData.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 CustomerPortalSubscriptionAddon.update_forward_refs()
-CustomerPortalSubscriptionPriceFragment.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentPrice.update_forward_refs()
-CustomerPortalSubscriptionPriceFragmentFeature.update_forward_refs()
 CustomerPortalSubscriptionFragment.update_forward_refs()
 CustomerPortalSubscriptionFragmentPrices.update_forward_refs()
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
-CustomerResourceFragment.update_forward_refs()
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
+TotalPriceFragment.update_forward_refs()
+TotalPriceFragmentSubTotal.update_forward_refs()
+TotalPriceFragmentTotal.update_forward_refs()
 SubscriptionScheduledUpdateData.update_forward_refs()
 SubscriptionScheduledUpdateDataTargetPackage.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesBillingPeriodChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesDowngradeChangeVariables.update_forward_refs()
 SubscriptionScheduledUpdateDataScheduleVariablesUnitAmountChangeVariables.update_forward_refs()
 SubscriptionFragment.update_forward_refs()
 SubscriptionFragmentResource.update_forward_refs()
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_active_subscriptions.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_active_subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import List
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_coupons.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_coupons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import CouponFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_customer_by_id.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_customer_by_id.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_customer_portal_by_ref_id.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_customer_portal_by_ref_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import CustomerPortalFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_mock_paywall.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_mock_paywall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_products.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_products.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import List
 
 from .base_model import BaseModel
 from .fragments import ProductFragment
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/get_sdk_configuration.py` & `stigg_api_client_v2-0.496.0/stigg/generated/get_sdk_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/input_types.py` & `stigg_api_client_v2-0.496.0/stigg/generated/input_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: ../api-client-schema/src/generated/schema.graphql
 
 from typing import Any, List, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/migrate_subscription_to_latest.py` & `stigg_api_client_v2-0.496.0/stigg/generated/migrate_subscription_to_latest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/provision_customer.py` & `stigg_api_client_v2-0.496.0/stigg/generated/provision_customer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/provision_subscription.py` & `stigg_api_client_v2-0.496.0/stigg/generated/provision_subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/report_usage.py` & `stigg_api_client_v2-0.496.0/stigg/generated/report_usage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from typing import Any, Optional
 
 from pydantic import Field
 
 from .base_model import BaseModel
```

### Comparing `stigg_api_client_v2-0.493.0/stigg/generated/update_subscription.py` & `stigg_api_client_v2-0.496.0/stigg/generated/update_subscription.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by ariadne-codegen on 2023-07-19 06:42
+# Generated by ariadne-codegen on 2023-07-20 15:44
 # Source: operations.graphql
 
 from pydantic import Field
 
 from .base_model import BaseModel
 from .fragments import SlimSubscriptionFragment
```

### Comparing `stigg_api_client_v2-0.493.0/PKG-INFO` & `stigg_api_client_v2-0.496.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stigg-api-client-v2
-Version: 0.493.0
+Version: 0.496.0
 Summary: 
 Author: Stigg
 Author-email: support@stigg.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

