# Comparing `tmp/pyroostermoney-0.2.1.tar.gz` & `tmp/pyroostermoney-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.2.1.tar", last modified: Mon Jul 17 20:15:04 2023, max compression
+gzip compressed data, was "pyroostermoney-0.2.2.tar", last modified: Thu Jul 20 13:16:51 2023, max compression
```

## Comparing `pyroostermoney-0.2.1.tar` & `pyroostermoney-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.574169 pyroostermoney-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.566169 pyroostermoney-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.570169 pyroostermoney-0.2.1/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.570169 pyroostermoney-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-17 20:15:04.574169 pyroostermoney-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.570169 pyroostermoney-0.2.1/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.574169 pyroostermoney-0.2.1/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/child/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/child/standing_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/child/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:15:04.570169 pyroostermoney-0.2.1/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-17 20:15:04.000000 pyroostermoney-0.2.1/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 20:15:04.000000 pyroostermoney-0.2.1/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:15:04.000000 pyroostermoney-0.2.1/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 20:15:04.000000 pyroostermoney-0.2.1/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 20:15:04.000000 pyroostermoney-0.2.1/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 20:15:04.574169 pyroostermoney-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-17 20:14:50.000000 pyroostermoney-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.394360 pyroostermoney-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.394360 pyroostermoney-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.394360 pyroostermoney-0.2.2/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8593 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/standing_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/child/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 13:16:51.000000 pyroostermoney-0.2.2/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-20 13:16:51.398360 pyroostermoney-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 13:16:38.000000 pyroostermoney-0.2.2/setup.py
```

### Comparing `pyroostermoney-0.2.1/.github/workflows/build.yml` & `pyroostermoney-0.2.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.1/.gitignore` & `pyroostermoney-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.1/LICENSE` & `pyroostermoney-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.1/PKG-INFO` & `pyroostermoney-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.1
+Version: 0.2.2
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/api.py` & `pyroostermoney-0.2.2/pyroostermoney/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Rooster Money requests and session handler."""
-
+# pylint: disable=too-many-arguments
+# pylint: disable=too-many-branches
+# pylint: disable=too-many-arguments
+# pylint: disable=too-many-instance-attributes
 import json
 import logging
 import base64
 import asyncio
 from datetime import datetime, timedelta
 
 import aiohttp
 
 from .const import HEADERS, BASE_URL, LOGIN_BODY, URLS
 from .exceptions import InvalidAuthError, NotLoggedIn, AuthenticationExpired
+from .events import Events
 
 _LOGGER = logging.getLogger(__name__)
 
 async def _fetch_request(url, headers=None):
     if headers is None:
         headers=HEADERS
     async with aiohttp.ClientSession() as session:
@@ -51,21 +55,26 @@
                 "status": response.status,
                 "response": json.loads(text)
             }
 
 class RoosterSession:
     """The main Rooster Session."""
 
-    def __init__(self, username: str, password: str, update_interval: int=30, use_updater: bool=False) -> None:
+    def __init__(self,
+                 username: str,
+                 password: str,
+                 update_interval: int=30,
+                 use_updater: bool=False) -> None:
         self._username = username
         self._password = password
         self._session = None
         self._headers = HEADERS
         self._logged_in = False
         self._logging_in = asyncio.Lock()
+        self.events = Events()
         self.update_interval = update_interval
         self.use_updater = use_updater
 
     async def async_login(self):
         """Logs into RoosterMoney and starts a new active session."""
         if self._logging_in.locked():
             _LOGGER.warning("Login already attempting. Only one execution allowed.")
@@ -124,57 +133,58 @@
                                         method="GET",
                                         login_request=False,
                                         add_security_token=False):
         """Handles all incoming requests to make sure that the session is active."""
 
         if self._session is None and self._logged_in:
             raise RuntimeError("Invalid state. Missing session data yet currently logged in?")
-        elif self._session is None and self._logged_in is False and auth is not None:
+        if self._session is None and self._logged_in is False and auth is not None:
             _LOGGER.info("Not logged in, trying now.")
             if headers is None:
                 headers = self._headers
             return await _post_request(url, body, auth, headers)
-        elif self._session is None and self._logged_in is False and auth is None:
+        if self._session is None and self._logged_in is False and auth is None:
             raise NotLoggedIn()
-        elif self._session is not None and self._logged_in is False:
+        if self._session is not None and self._logged_in is False:
             raise RuntimeError("Invalid state. Session data available yet not logged in?")
-        elif self._session["expiry_time"] < datetime.now() and login_request:
+        if self._session["expiry_time"] < datetime.now() and login_request:
             _LOGGER.debug("Login request.")
             return await _post_request(url, body, auth, headers)
 
         # Check if auth has expired
-
+        # pylint: disable=no-else-raise
+        # pylint: disable=no-else-return
         if self._session["expiry_time"] < datetime.now():
             raise AuthenticationExpired()
 
         if headers is None:
             headers = self._headers
 
         if add_security_token:
             headers["securitytoken"] = self._session["security_code"]
 
         if method == "GET":
             return await _fetch_request(url, headers=headers)
-        elif method == "POST":
+        if method == "POST":
             return await _post_request(url, body=body, headers=headers)
-        elif method == "DELETE":
+        if method == "DELETE":
             return await _delete_request(url, body=body, headers=headers)
         else:
             raise ValueError("Invalid type argument.")
 
     async def request_handler(self,
                                         url,
                                         body=None,
                                         headers=None,
                                         auth=None,
                                         method="GET",
                                         login_request=False,
                                         add_security_token=False):
         """Public calls for the private _internal_request_handler."""
-        _LOGGER.debug(f"Sending {method} HTTP request to {url}")
+        _LOGGER.debug("Sending %s HTTP request to %s", method, url)
         try:
             return await self._internal_request_handler(
                 url=url,
                 body=body,
                 headers=headers,
                 auth=auth,
                 method=method,
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/child/__init__.py` & `pyroostermoney-0.2.2/pyroostermoney/child/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,99 +1,91 @@
 """Defines some standard values for a Natwest Rooster Money child."""
-
-import asyncio, logging
-from datetime import datetime, timedelta, date
+# pylint: disable=too-many-instance-attributes
+import logging
+from datetime import datetime, date
 
 from pyroostermoney.const import URLS
 from pyroostermoney.api import RoosterSession
-from .money_pot import Pot, convert_response as MoneyPotConverter
+from pyroostermoney.events import EventSource, EventType
+from .money_pot import Pot
 from .card import Card
-from .standing_order import StandingOrder, convert_response as StandingOrderConverter
+from .standing_order import StandingOrder
 from .jobs import Job
 from .transaction import Transaction
 
 _LOGGER = logging.getLogger(__name__)
 
 class ChildAccount:
     """The child account."""
 
-    def __init__(self, raw_response: dict, session: RoosterSession) -> None:
+    def __init__(self, raw_response: dict, session: RoosterSession, exclude_card = False) -> None:
         self._parse_response(raw_response)
         self._session = session
         self.pots: list[Pot] = []
         self.card: Card = None
         self.standing_orders: list[StandingOrder] = []
         self.jobs: list[Job] = []
         self.active_allowance_period_id: int = None
         self.transactions: list[Transaction] = []
         self.latest_transaction: Transaction = None
-        self._exclude_card = False
-        self._update_lock = asyncio.Lock()
-        if self._session.use_updater:
-            _LOGGER.debug("Using auto updater for ChildAccount")
-            self._updater = asyncio.create_task(self._update_scheduler())
-        self.last_updated = datetime.now()
+        self._exclude_card = exclude_card
 
     def __del__(self):
-        if self._session.use_updater:
-            self._updater.cancel()
-            self._updater = None
+        pass
+        # if self._session.use_updater:
+        #     self._updater.cancel()
+        #     self._updater = None
 
     def __eq__(self, obj):
         if not isinstance(obj, ChildAccount):
             return NotImplemented
 
         return (self.available_pocket_money == obj.available_pocket_money
         ) and (self.jobs == obj.jobs) and (self.pots == obj.pots) and (
             self.active_allowance_period_id == obj.active_allowance_period_id
         )
 
-    async def _update_scheduler(self):
-        """Async auto update loop."""
-        while True:
-            next_time = datetime.now() + timedelta(seconds=self._session.update_interval)
-            while datetime.now() < next_time:
-                await asyncio.sleep(1)
-            await self.update()
-
     async def perform_init(self):
         """Performs init for some internal async props."""
         await self.get_pocket_money()
         if not self._exclude_card:
             await self.get_card_details()
             self._exclude_card=True
         await self.get_standing_orders()
         await self.get_active_allowance_period()
         await self.get_current_jobs()
         await self.get_spend_history()
 
     async def update(self):
         """Updates the cached data for this child."""
+        p_self = self
         _LOGGER.debug("Update ChildAccount")
-        if self._update_lock.locked():
-            return True
-
-        async with self._update_lock:
-            response = await self._session.request_handler(
-                url=URLS.get("get_child").format(user_id=self.user_id))
-            self._parse_response(response)
-            await self.perform_init()
-            self.last_updated = datetime.now()
+        response = await self._session.request_handler(
+            url=URLS.get("get_child").format(user_id=self.user_id))
+        self._parse_response(response)
+        await self.perform_init()
+        if (p_self is not None and
+            p_self.active_allowance_period_id != self.active_allowance_period_id or
+            p_self.available_pocket_money != self.available_pocket_money):
+            self._session.events.fire_event(EventSource.CHILD, EventType.UPDATED,
+                                            {
+                                                "user_id": self.user_id
+                                            })
 
     def _parse_response(self, raw_response:dict):
         """Parses the raw_response into this object"""
         if "response" in raw_response:
             raw_response = raw_response["response"]
         self.interest_rate = raw_response["interestRate"]
         self.available_pocket_money = raw_response["availablePocketMoney"]
         self.currency = raw_response["currency"]
         self.first_name = raw_response["firstName"]
         self.surname = raw_response["surname"]
         self.gender = "male" if raw_response["gender"] == 1 else "female"
-        self.uses_real_money = True if raw_response["realMoneyStatus"] == 1 else False
+        self.uses_real_money = raw_response["realMoneyStatus"] == 1
         self.user_id = raw_response["userId"]
         self.profile_image = raw_response["profileImageUrl"]
 
     async def get_active_allowance_period(self):
         """Returns the current active allowance period."""
         allowance_periods = await self._session.request_handler(
             url=URLS.get("get_child_allowance_periods").format(user_id=self.user_id))
@@ -114,20 +106,33 @@
         """Gets the spend history"""
         url = URLS.get("get_child_spend_history").format(
             user_id=self.user_id,
             count=count
         )
         response = await self._session.request_handler(url=url)
         self.transactions = Transaction.parse_response(response["response"])
+        p_transaction = self.latest_transaction
         self.latest_transaction = self.transactions[len(self.transactions)-1]
+        if (p_transaction is not None
+            and self.latest_transaction.transaction_id != p_transaction.transaction_id):
+            self._session.events.fire_event(EventSource.TRANSACTIONS, EventType.UPDATED, {
+                "old_transaction_id": p_transaction.transaction_id,
+                "new_transaction_id": self.latest_transaction.transaction_id
+            })
         return self.transactions
 
     async def get_current_jobs(self) -> list[Job]:
         """Gets jobs for the current allowance period."""
+        p_jobs = self.jobs
         self.jobs = await self.get_allowance_period_jobs(self.active_allowance_period_id)
+        if (len(p_jobs) > 0 and
+            self.jobs[len(self.jobs)-1].master_job_id != p_jobs[len(p_jobs)-1].master_job_id):
+            self._session.events.fire_event(EventSource.JOBS, EventType.UPDATED, {
+                "job_length": [len(self.jobs)]
+            })
         return self.jobs
 
     async def get_allowance_period_jobs(self, allowance_period_id):
         """Gets jobs for a given allowance period"""
         url = URLS.get("get_child_allowance_period_jobs").format(
             user_id=self.user_id,
             allowance_period_id=allowance_period_id
@@ -138,15 +143,15 @@
 
     async def get_pocket_money(self):
         """Gets pocket money"""
         url = URLS.get("get_child_pocket_money").format(
             user_id=self.user_id
         )
         response = await self._session.request_handler(url)
-        self.pots: list[Pot] = MoneyPotConverter(response["response"])
+        self.pots: list[Pot] = Pot.convert_response(response["response"])
 
         return self.pots
 
     async def special_get_pocket_money(self):
         """Same as get_pocket_money yet parses the response and provides a basic dict."""
         pocket_money = await self.get_pocket_money()
 
@@ -162,76 +167,68 @@
         """Returns the card details for the child."""
         card_details = await self._session.request_handler(
             URLS.get("get_child_card_details").format(
                 user_id=self.user_id
             )
         )
 
-        self.card = Card(card_details["response"], self.user_id, self._session)
+        self.card = Card.parse_response(card_details["response"], self.user_id, self._session)
         await self.card.init_card_pin()
         return self.card
 
     async def get_standing_orders(self) -> list[StandingOrder]:
         """Returns a list of standing orders for the child."""
         standing_orders = await self._session.request_handler(
             URLS.get("get_child_standing_orders").format(
                 user_id=self.user_id
             )
         )
+        p_standing_orders = self.standing_orders
+        self.standing_orders = StandingOrder.convert_response(standing_orders)
+        if (len(p_standing_orders)>0 and
+            p_standing_orders[len(p_standing_orders)-1].regular_id is not
+            self.standing_orders[len(self.standing_orders)-1].regular_id):
+            self._session.events.fire_event(EventSource.STANDING_ORDER, EventType.UPDATED, {
+                "new_regular_id": self.standing_orders[len(self.standing_orders)-1].regular_id,
+                "old_regular_id": p_standing_orders[len(p_standing_orders)-1].regular_id
+            })
 
-        self.standing_orders = StandingOrderConverter(standing_orders)
         return self.standing_orders
 
-    async def add_to_pot(self, value: float, target: Pot) -> Pot:
-        """Add money to a pot."""
-        # TODO
-        pass
+    # async def add_to_pot(self, value: float, target: Pot) -> Pot:
+    #     """Add money to a pot."""
 
-    async def remove_from_pot(self, value: float, target: Pot) -> Pot:
-        """Remove money from a pot"""
-        # TODO
-        pass
+    # async def remove_from_pot(self, value: float, target: Pot) -> Pot:
+    #     """Remove money from a pot"""
 
-    async def transfer_money(self, value: float, source: Pot, target: Pot) -> Pot:
-        """Transfers money between two pots."""
-        # TODO
-        pass
+    # async def transfer_money(self, value: float, source: Pot, target: Pot) -> Pot:
+    #     """Transfers money between two pots."""
 
-    async def create_pot(self, new_pot: Pot) -> Pot:
-        """Create a new pot."""
-        # TODO
-        pass
+    # async def create_pot(self, new_pot: Pot) -> Pot:
+    #     """Create a new pot."""
 
-    async def delete_pot(self, pot: Pot) -> bool:
-        """Delete a pot."""
-        # TODO
-        return True
+    # async def delete_pot(self, pot: Pot) -> bool:
+    #     """Delete a pot."""
 
     async def create_standing_order(self, standing_order: StandingOrder):
         """Create a standing order."""
         output = await self._session.request_handler(
             URLS.get("create_child_standing_order").format(
                 user_id=self.user_id
             ),
             standing_order.__dict__,
             method="POST"
         )
 
-        if output.get("status") == 200:
-            return True
-        else:
-            return False
+        return bool(output.get("status") == 200)
 
     async def delete_standing_order(self, standing_order: StandingOrder):
         """Delete a standing order."""
         output = await self._session.request_handler(
             URLS.get("delete_child_standing_order").format(
                 user_id=self.user_id,
                 standing_order_id=standing_order.regular_id
             ),
             method="DELETE"
         )
 
-        if output.get("status") == 200:
-            return True
-        else:
-            return False
+        return bool(output.get("status") == 200)
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/child/jobs.py` & `pyroostermoney-0.2.2/pyroostermoney/child/jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Job type."""
-
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-locals
+# pylint: disable=too-many-arguments
 from datetime import datetime
 from enum import Enum
 
 from pyroostermoney.api import RoosterSession
 from pyroostermoney.const import CURRENCY
 
 class JobState(Enum):
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.2.2/pyroostermoney/child/money_pot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Defines a money pot."""
-
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
+# pylint: disable=too-few-public-methods
 from datetime import datetime
 
 from pyroostermoney.const import SPEND_POT_ID, SAVINGS_POT_ID, GIVE_POT_ID, GOAL_POT_ID
 
 class Pot:
     """A money pot."""
 
@@ -21,64 +23,64 @@
         self.pot_id = pot_id
         self.image = image
         self.enabled = enabled
         self.value = value
         self.target = target
         self.last_updated = last_updated
 
+    @staticmethod
+    def convert_response(raw: dict) -> list['Pot']:
+        """Converts a raw response into a list of Pot"""
+        output: list[Pot] = []
+
+        # process the default pots first, starting with savings
+        savings = Pot(name="Savings",
+                    ledger=None,
+                    pot_id=SAVINGS_POT_ID,
+                    image=None,
+                    enabled=raw["potSettings"]["savePot"]["display"],
+                    value=raw["safeTotal"],
+                    target=raw["saveGoalAmount"])
+        output.append(savings)
+
+        # goal pot
+        goals = Pot(name="Goals",
+                    ledger=None,
+                    pot_id=GOAL_POT_ID,
+                    image=None,
+                    enabled=raw["potSettings"]["goalPot"]["display"],
+                    value=raw["allocatedToGoals"])
+        output.append(goals)
+
+        # spend pot
+        goals = Pot(name="Spending",
+                    ledger=None,
+                    pot_id=SPEND_POT_ID,
+                    image=None,
+                    enabled=raw["potSettings"]["spendPot"]["display"],
+                    value=raw["walletTotal"])
+        output.append(goals)
+
+        # spend pot
+        goals = Pot(name="Give",
+                    ledger=None,
+                    pot_id=GIVE_POT_ID,
+                    image=None,
+                    enabled=raw["potSettings"]["givePot"]["display"],
+                    value=raw["giveAmount"])
+        output.append(goals)
+
+        # now process custom pots
+        for pot in raw["customPots"]:
+            custom_pot = Pot(
+                name=pot["customLedgerMetadata"]["title"],
+                pot_id=pot["customPotId"],
+                ledger=pot["customLedgerMetadata"],
+                image=pot["customLedgerMetadata"]["imageUrl"],
+                enabled=True, # custom pots enabled by default
+                value=pot["availableBalance"]["amount"],
+                target=pot["customLedgerMetadata"]["upperLimit"]["amount"],
+                last_updated=pot["updated"]
+            )
+            output.append(custom_pot)
 
-def convert_response(raw: dict) -> list[Pot]:
-    """Converts a raw response into a list of Pot"""
-    output: list[Pot] = []
-
-    # process the default pots first, starting with savings
-    savings = Pot(name="Savings",
-                  ledger=None,
-                  pot_id=SAVINGS_POT_ID,
-                  image=None,
-                  enabled=raw["potSettings"]["savePot"]["display"],
-                  value=raw["safeTotal"],
-                  target=raw["saveGoalAmount"])
-    output.append(savings)
-
-    # goal pot
-    goals = Pot(name="Goals",
-                  ledger=None,
-                  pot_id=GOAL_POT_ID,
-                  image=None,
-                  enabled=raw["potSettings"]["goalPot"]["display"],
-                  value=raw["allocatedToGoals"])
-    output.append(goals)
-
-    # spend pot
-    goals = Pot(name="Spending",
-                  ledger=None,
-                  pot_id=SPEND_POT_ID,
-                  image=None,
-                  enabled=raw["potSettings"]["spendPot"]["display"],
-                  value=raw["walletTotal"])
-    output.append(goals)
-
-    # spend pot
-    goals = Pot(name="Give",
-                  ledger=None,
-                  pot_id=GIVE_POT_ID,
-                  image=None,
-                  enabled=raw["potSettings"]["givePot"]["display"],
-                  value=raw["giveAmount"])
-    output.append(goals)
-
-    # now process custom pots
-    for pot in raw["customPots"]:
-        custom_pot = Pot(
-            name=pot["customLedgerMetadata"]["title"],
-            pot_id=pot["customPotId"],
-            ledger=pot["customLedgerMetadata"],
-            image=pot["customLedgerMetadata"]["imageUrl"],
-            enabled=True, # custom pots enabled by default
-            value=pot["availableBalance"]["amount"],
-            target=pot["customLedgerMetadata"]["upperLimit"]["amount"],
-            last_updated=pot["updated"]
-        )
-        output.append(custom_pot)
-
-    return output
+        return output
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/child/standing_order.py` & `pyroostermoney-0.2.2/pyroostermoney/child/standing_order.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A standing order."""
+# pylint: disable=too-many-arguments
 
 class StandingOrder:
     """A standing order."""
 
     def __init__(self,
                  amount: float,
                  day: str,
@@ -24,26 +25,27 @@
             "amount": str(self.amount),
             "day": self.day,
             "frequency": self.frequency,
             "tag": self.tag,
             "title": self.title
         }
 
-def convert_response(raw_response: str) -> list[StandingOrder]:
-    """Parses a raw response of standing orders into a list of StandingOrder"""
-    output: list[StandingOrder] = []
-    if "response" in raw_response:
-        raw_response = raw_response["response"]
-
-    for regular in raw_response:
-        standing_order = StandingOrder(
-            amount=float(regular.get("amount")),
-            day=regular.get("day"),
-            frequency=regular.get("frequency"),
-            regular_id=regular.get("id"),
-            active=True if regular.get("paused") is False else False,
-            tag=regular.get("tag"),
-            title=regular.get("title")
-        )
-        output.append(standing_order)
+    @staticmethod
+    def convert_response(raw_response: str) -> list['StandingOrder']:
+        """Parses a raw response of standing orders into a list of StandingOrder"""
+        output: list[StandingOrder] = []
+        if "response" in raw_response:
+            raw_response = raw_response["response"]
+
+        for regular in raw_response:
+            standing_order = StandingOrder(
+                amount=float(regular.get("amount")),
+                day=regular.get("day"),
+                frequency=regular.get("frequency"),
+                regular_id=regular.get("id"),
+                active= bool(regular.get("paused")) is not True,
+                tag=regular.get("tag"),
+                title=regular.get("title")
+            )
+            output.append(standing_order)
 
-    return output
+        return output
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/child/transaction.py` & `pyroostermoney-0.2.2/pyroostermoney/child/transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """A transaction class"""
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
 
 from datetime import datetime
 
 from pyroostermoney.const import CURRENCY
 
 
 class Transaction:
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/const.py` & `pyroostermoney-0.2.2/pyroostermoney/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.2.1"
+VERSION="0.2.2"
 BASE_URL="https://api.rooster.money"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/exceptions.py` & `pyroostermoney-0.2.2/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.1/pyroostermoney/family_account.py` & `pyroostermoney-0.2.2/pyroostermoney/family_account.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # pylint: disable=fixme
 """Defines the class for the family account."""
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
 
-import asyncio, logging
-from datetime import datetime, timedelta
+import asyncio
+import logging
+from datetime import datetime
 
 from .api import RoosterSession
 from .const import URLS, DEFAULT_BANK_NAME, DEFAULT_BANK_TYPE, CREATE_PAYMENT_BODY, CURRENCY
+from .events import EventType, EventSource
 
 _LOGGER = logging.getLogger(__name__)
 
 class FamilyAccount:
     """A family account."""
 
     def __init__(self,
                  raw_response: dict,
                  account_info: dict,
                  session: RoosterSession) -> None:
         self._session = session
         self._parse_response(raw_response, account_info)
         self._update_lock = asyncio.Lock()
-        if self._session.use_updater:
-            _LOGGER.debug("Using auto updater for FamilyAccount")
-            self._updater = asyncio.create_task(self._update_scheduler())
         self.last_updated = datetime.now()
 
-    def __del__(self):
-        if self._session.use_updater:
-            self._updater.cancel()
-            self._updater = None
-
     def _parse_response(self, raw_response: dict, account_info: dict):
         """Parses the raw response."""
         _LOGGER.debug("Parsing new response")
         if "response" in raw_response:
             raw_response = raw_response["response"]
 
         self.account_number = raw_response["accountNumber"]
@@ -41,36 +37,33 @@
         amount = raw_response["suggestedMonthlyTransfer"]["amount"]
         self.suggested_monthly_transfer = amount / (1 * 10**self._precision)
         self.currency = raw_response["suggestedMonthlyTransfer"]["currency"]
         self.balance = account_info.get("familyLedgerBalance", None)
         if self.balance is not None:
             self.balance = float(self.balance)
 
-    async def _update_scheduler(self):
-        """Automatic updates according to the update interval."""
-        while True:
-            next_time = datetime.now() + timedelta(seconds=self._session.update_interval)
-            while datetime.now() < next_time:
-                await asyncio.sleep(1)
-            _LOGGER.info("Updating data.")
-            await self.update()
-
     async def update(self):
         """Updates the FamilyAccount object data."""
         if self._update_lock.locked():
             return True
 
         async with self._update_lock:
             family_account = await self._session.request_handler(
                 url=URLS.get("get_family_account"))
             account = await self._session.request_handler(
                 url=URLS.get("get_account_info")
             )
+            p_account = self.__dict__
             self._parse_response(raw_response=family_account, account_info=account)
             self.last_updated = datetime.now()
+            if p_account is not self.__dict__:
+                self._session.events.fire_event(EventSource.FAMILY_ACCOUNT, EventType.UPDATED,
+                                                {
+                                                    "user_id": self.account_number
+                                                })
 
     @property
     def bank_transfer_details(self):
         """Gets the bank transfer details to top up the family account."""
         return {
             "account_number": self.account_number,
             "sort_code": self.sort_code,
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney/roostermoney.py` & `pyroostermoney-0.2.2/pyroostermoney/roostermoney.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,110 @@
 """The RoosterMoney integration."""
+# pylint: disable=too-many-instance-attributes
+# pylint: disable=too-many-arguments
 
-import logging, asyncio
+import logging
+import asyncio
 from datetime import datetime, timedelta
 
 from .const import URLS
 from .child import ChildAccount, Job
 from .family_account import FamilyAccount
 from .api import RoosterSession
+from .events import EventSource, EventType
 
 _LOGGER = logging.getLogger(__name__)
 
 class RoosterMoney(RoosterSession):
     """The RoosterMoney module."""
 
-    def __init__(self, username: str, password: str, update_interval: int=30, use_updater: bool=False) -> None:
+    def __init__(self,
+                 username: str,
+                 password: str,
+                 update_interval: int=30,
+                 use_updater: bool=False,
+                 remove_card_information = False) -> None:
         super().__init__(
             username=username,
             password=password,
             use_updater=use_updater,
             update_interval=update_interval
         )
         self.account_info = None
         self.children: list[ChildAccount] = []
         self.master_job_list: list[Job] = []
         self._discovered_children: list = []
         self.family_account: FamilyAccount = None
         self._update_lock = asyncio.Lock()
         self._updater = None
+        self._remove_card_information = remove_card_information
+        self._init = True
 
     def __del__(self):
         if self.use_updater:
             self._updater.cancel()
             self._updater = None
 
     async def async_login(self):
         await super().async_login()
-        await self.update()
         await self.get_family_account()
+        await self.update()
         if self.use_updater:
-            _LOGGER.debug("Using built-in updater for RoosterMoney")
+            _LOGGER.debug("Using auto updater for RoosterMoney")
             self._updater = asyncio.create_task(self._update_scheduler())
+        self._init = False
 
     async def _update_scheduler(self):
         """Automatic updater"""
         while True:
             next_time = datetime.now() + timedelta(seconds=self.update_interval)
             while datetime.now() < next_time:
                 await asyncio.sleep(1)
-            _LOGGER.info("Updating data")
             await self.update()
 
     async def update(self):
         """Perform an update of all root types"""
         if self._update_lock.locked():
             return True
 
         async with self._update_lock:
             await self.get_children()
             await self.get_master_job_list()
+            for child in self.children:
+                await child.update()
+            await self.family_account.update()
 
     async def get_children(self) -> list[ChildAccount]:
         """Returns a list of available children."""
         account_info = await self.get_account_info()
         children = account_info["children"]
         for child in children:
             if child.get("userId") not in self._discovered_children:
-                child = ChildAccount(child, self)
+                child = ChildAccount(child, self, self._remove_card_information)
                 await child.perform_init() # calling this will init some extra props.
                 self._discovered_children.append(child.user_id)
                 self.children.append(child)
+                self.events.fire_event(EventSource.CHILD, EventType.CREATED, {
+                    "user_id": child.user_id
+                })
         _LOGGER.debug(self._discovered_children)
+        self._cleanup()
         return self.children
 
+    def _cleanup(self) -> None:
+        """Removes data that no longer exists from the updater."""
+        for i in range(len(self.children)):
+            child_id = self.children[i-1].user_id
+            if child_id not in self._discovered_children:
+                _LOGGER.debug("child %s no longer exists at source", child_id)
+                self.children.pop(i-1)
+                self.events.fire_event(EventSource.CHILD, EventType.DELETED, {
+                    "user_id": child_id
+                })
+
     async def get_account_info(self) -> dict:
         """Returns the account info for the current user."""
         self.account_info = await self.request_handler(url=URLS.get("get_account_info"))
         self.account_info = self.account_info["response"]
         return self.account_info
 
     def get_child_account(self, user_id) -> ChildAccount:
```

### Comparing `pyroostermoney-0.2.1/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.2.2/pyroostermoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.1
+Version: 0.2.2
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

