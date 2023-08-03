# Comparing `tmp/pyroostermoney-0.2.5.tar.gz` & `tmp/pyroostermoney-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroostermoney-0.2.5.tar", last modified: Wed Jul 26 16:41:17 2023, max compression
+gzip compressed data, was "pyroostermoney-0.3.0.tar", last modified: Thu Aug  3 23:08:35 2023, max compression
```

## Comparing `pyroostermoney-0.2.5.tar` & `pyroostermoney-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/pyroostermoney/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8799 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/pyroostermoney/child/
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/money_pot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/standing_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/child/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/family_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/master_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/pyroostermoney/roostermoney.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 16:41:17.943302 pyroostermoney-0.2.5/pyroostermoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 16:41:17.000000 pyroostermoney-0.2.5/pyroostermoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 16:41:17.947302 pyroostermoney-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-26 16:41:06.000000 pyroostermoney-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:08:35.229992 pyroostermoney-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/pyroostermoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/pyroostermoney/child/
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/child/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/child/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/child/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/child/money_pot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/child/standing_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/child/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/family_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/master_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/pyroostermoney/roostermoney.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/pyroostermoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-03 23:08:35.000000 pyroostermoney-0.3.0/pyroostermoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-03 23:08:35.000000 pyroostermoney-0.3.0/pyroostermoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:08:35.000000 pyroostermoney-0.3.0/pyroostermoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-03 23:08:35.000000 pyroostermoney-0.3.0/pyroostermoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-03 23:08:35.000000 pyroostermoney-0.3.0/pyroostermoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-08-03 23:08:35.233992 pyroostermoney-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-08-03 23:08:24.000000 pyroostermoney-0.3.0/setup.py
```

### Comparing `pyroostermoney-0.2.5/.github/workflows/build.yml` & `pyroostermoney-0.3.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/.gitignore` & `pyroostermoney-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/LICENSE` & `pyroostermoney-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/PKG-INFO` & `pyroostermoney-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.5
+Version: 0.3.0
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.5/cli.py` & `pyroostermoney-0.3.0/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,16 +17,17 @@
     selected_child = None
     while logged_in is not True:
         _LOGGER.debug("Login required")
         username = input("Please enter your username: ")
         password = input("Please enter your password: ")
         card_info = input("Collect card information? [Y/n] ")
         try:
-            session = RoosterMoney(username, password, remove_card_information=card_info=="n")
-            await session.async_login()
+            session = await RoosterMoney.create(username,
+                                                password,
+                                                remove_card_information=card_info=="n")
             print("Logged in as ", username)
             logged_in = True
         except PermissionError:
             print("Username or password incorrect")
 
     while logged_in:
         try:
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/api.py` & `pyroostermoney-0.3.0/pyroostermoney/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,20 +16,18 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 class RoosterSession:
     """The main Rooster Session."""
 
     def __init__(self,
-                 username: str,
-                 password: str,
                  update_interval: int=30,
                  use_updater: bool=False) -> None:
-        self._username = username
-        self._password = password
+        self._username = ""
+        self._password = ""
         self._session = None
         self._headers = HEADERS
         self._logged_in = False
         self._logging_in = asyncio.Lock()
         self.events = Events()
         self.update_interval = update_interval
         self.use_updater = use_updater
@@ -77,23 +75,25 @@
                 "refresh_token": login_response.get("refresh_token"),
                 "token_type": token_type,
                 "expiry_time": datetime.now() + timedelta(0,
                                                           login_response.get("expires_in")),
                 "security_code": token
             }
 
-    async def async_login(self):
+    async def _session_start(self, username, password):
         """Logs into RoosterMoney and starts a new active session."""
         if self._logging_in.locked():
             _LOGGER.warning("Login already attempting. Only one execution allowed.")
             while self._logging_in.locked():
                 await asyncio.sleep(1)
             return True
 
         async with self._logging_in:
+            self._username = username
+            self._password = password
             if self._session is not None:
                 if self._session.get("expiry_time") > datetime.now():
                     _LOGGER.debug("Not logging in again, session already active.")
                     return True
 
             req_body = LOGIN_BODY
             req_body["username"] = self._username
@@ -128,15 +128,15 @@
             form.add_field("client_id", "rooster-app")
             form.add_field("refresh_token", self._session.get("refresh_token"))
             try:
                 async with session.post(OAUTH_TOKEN_URL, data=form) as request:
                     data = await request.json()
                     self._session = self._parse_login(data, self._session.get("security_code"))
             except ConnectionError:
-                await self.async_login()
+                await self._session_start(self._username, self._password)
 
     async def _internal_request_handler(self,
                                         url,
                                         body=None,
                                         auth=None,
                                         method="GET",
                                         login_request=False,
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/child/__init__.py` & `pyroostermoney-0.3.0/pyroostermoney/child/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,72 +1,101 @@
 """Defines some standard values for a Natwest Rooster Money child."""
 # pylint: disable=too-many-instance-attributes
 import logging
-from datetime import datetime, date
+import asyncio
+from datetime import datetime, date, timedelta
 
-from pyroostermoney.const import URLS
+from pyroostermoney.const import URLS, CHILD_MAX_TRANSACTION_COUNT
 from pyroostermoney.api import RoosterSession
 from pyroostermoney.events import EventSource, EventType
 from .money_pot import Pot
 from .card import Card
 from .standing_order import StandingOrder
 from .jobs import Job
 from .transaction import Transaction
 
 _LOGGER = logging.getLogger(__name__)
 
 class ChildAccount:
     """The child account."""
 
-    def __init__(self, raw_response: dict, session: RoosterSession, exclude_card = False) -> None:
-        self._parse_response(raw_response)
+    def __init__(self, user_id: int,
+                 session: RoosterSession,
+                 exclude_card_pin = False) -> None:
+        self._exclude_card_pin = exclude_card_pin
         self._session = session
+        self._update_lock = asyncio.Lock()
+        self._updater: asyncio.Task = None
+        self.user_id = user_id
+        self.interest_rate = None
+        self.available_pocket_money = None
+        self.currency = None
+        self.first_name = None
+        self.surname = None
+        self.gender = None
+        self.uses_real_money = -1
+        self.profile_image = ""
         self.pots: list[Pot] = []
         self.card: Card = None
         self.standing_orders: list[StandingOrder] = []
         self.jobs: list[Job] = []
         self.active_allowance_period_id: int = None
         self.transactions: list[Transaction] = []
+        self.declined_transactions: list[Transaction] = []
         self.latest_transaction: Transaction = None
-        self._exclude_card = exclude_card
 
     def __del__(self):
-        pass
-        # if self._session.use_updater:
-        #     self._updater.cancel()
-        #     self._updater = None
+        _LOGGER.debug("Delete ChildAccount")
+        if self._session.use_updater:
+            self._updater.cancel()
+            self._updater = None
 
     def __eq__(self, obj):
         if not isinstance(obj, ChildAccount):
             return NotImplemented
 
         return (self.available_pocket_money == obj.available_pocket_money
         ) and (self.jobs == obj.jobs) and (self.pots == obj.pots) and (
             self.active_allowance_period_id == obj.active_allowance_period_id
         )
 
-    async def perform_init(self):
-        """Performs init for some internal async props."""
+    @classmethod
+    async def create(cls,
+                     user_id: int,
+                     session: RoosterSession,
+                     exclude_card_pin = True) -> 'ChildAccount':
+        """Inits and creates a child account object."""
+        self = cls(user_id, session, exclude_card_pin)
+        await self._update()
+        if session.use_updater:
+            _LOGGER.debug("Using auto updater for ChildAccount")
+            self._updater = asyncio.create_task(self._update_scheduler())
+        return self
+
+
+    async def _update_scheduler(self):
+        """Automatic updater"""
+        while True:
+            next_time = datetime.now() + timedelta(seconds=self._session.update_interval)
+            while datetime.now() < next_time:
+                await asyncio.sleep(1)
+            await self._update()
+
+    async def _update(self):
+        """Updates the cached data for this child."""
+        p_self = self
+        _LOGGER.debug("Update ChildAccount")
+        self._parse_response(await self._session.request_handler(
+            url=URLS.get("get_child").format(user_id=self.user_id)))
         await self.get_pocket_money()
-        if not self._exclude_card:
-            await self.get_card_details()
-            self._exclude_card=True
+        await self.get_card_details()
         await self.get_standing_orders()
         await self.get_active_allowance_period()
         await self.get_current_jobs()
         await self.get_spend_history()
-
-    async def update(self):
-        """Updates the cached data for this child."""
-        p_self = self
-        _LOGGER.debug("Update ChildAccount")
-        response = await self._session.request_handler(
-            url=URLS.get("get_child").format(user_id=self.user_id))
-        self._parse_response(response)
-        await self.perform_init()
         if (p_self is not None and
             p_self.active_allowance_period_id != self.active_allowance_period_id or
             p_self.available_pocket_money != self.available_pocket_money):
             self._session.events.fire_event(EventSource.CHILD, EventType.UPDATED,
                                             {
                                                 "user_id": self.user_id
                                             })
@@ -78,15 +107,14 @@
         self.interest_rate = raw_response["interestRate"]
         self.available_pocket_money = raw_response["availablePocketMoney"]
         self.currency = raw_response["currency"]
         self.first_name = raw_response["firstName"]
         self.surname = raw_response["surname"]
         self.gender = "male" if raw_response["gender"] == 1 else "female"
         self.uses_real_money = raw_response["realMoneyStatus"] == 1
-        self.user_id = raw_response["userId"]
         self.profile_image = raw_response["profileImageUrl"]
 
     async def get_active_allowance_period(self):
         """Returns the current active allowance period."""
         allowance_periods = await self._session.request_handler(
             url=URLS.get("get_child_allowance_periods").format(user_id=self.user_id))
         allowance_periods = allowance_periods["response"]
@@ -98,30 +126,50 @@
             raise LookupError("No allowance period found")
 
         active_periods = active_periods[0]
         self.active_allowance_period_id = int(active_periods.get("allowancePeriodId"))
 
         return active_periods
 
-    async def get_spend_history(self, count=10) -> list[Transaction]:
-        """Gets the spend history"""
+    async def _update_spend_history(self, count=10):
+        """Internal update handler for the spend history"""
         url = URLS.get("get_child_spend_history").format(
             user_id=self.user_id,
             count=count
         )
         response = await self._session.request_handler(url=url)
         self.transactions = Transaction.parse_response(response["response"])
+        # declined transaction should be ignored as it did not complete
+        # therefore it doesn't count towards the "spend history"
+        self.declined_transactions = list(filter(lambda x: x.declined, self.transactions))
+        self.transactions = list(filter(lambda x: (x.declined is not True), self.transactions))
         p_transaction = self.latest_transaction
         self.latest_transaction = self.transactions[len(self.transactions)-1]
         if (p_transaction is not None
             and self.latest_transaction.transaction_id != p_transaction.transaction_id):
             self._session.events.fire_event(EventSource.TRANSACTIONS, EventType.UPDATED, {
                 "old_transaction_id": p_transaction.transaction_id,
-                "new_transaction_id": self.latest_transaction.transaction_id
+                "new_transaction_id": self.latest_transaction.transaction_id,
+                "declined": self.latest_transaction.declined,
+                "declined_reason": self.latest_transaction.declined_reason
             })
+
+    async def get_spend_history(self, count=10) -> list[Transaction]:
+        """Gets the spend history"""
+        await self._update_spend_history(count)
+        required = count
+        # increase count dynamically to ignore declines
+        while len(self.transactions) < required:
+            _LOGGER.debug("ChildAccount get_spend_history returned only %s events",
+                          len(self.transactions))
+            count += 1
+            await self._update_spend_history(count)
+            if count == CHILD_MAX_TRANSACTION_COUNT:
+                break
+
         return self.transactions
 
     async def get_current_jobs(self) -> list[Job]:
         """Gets jobs for the current allowance period."""
         p_jobs = self.jobs
         self.jobs = await self.get_allowance_period_jobs(self.active_allowance_period_id)
         if (len(p_jobs) > 0 and
@@ -161,21 +209,28 @@
             "spend": pocket_money["pocketMoneyAmount"],
             "save": pocket_money["safeTotal"],
             "give": pocket_money["giveAmount"]
         }
 
     async def get_card_details(self):
         """Returns the card details for the child."""
+        if self.card is not None:
+            await self.card.update_family_card_entry() # Only run the updater if already set
+            return self.card
+
         card_details = await self._session.request_handler(
             URLS.get("get_child_card_details").format(
                 user_id=self.user_id
             )
         )
 
         self.card = Card.parse_response(card_details["response"], self.user_id, self._session)
+        if self._exclude_card_pin is True:
+            return self.card
+
         await self.card.init_card_pin()
         return self.card
 
     async def get_standing_orders(self) -> list[StandingOrder]:
         """Returns a list of standing orders for the child."""
         standing_orders = await self._session.request_handler(
             URLS.get("get_child_standing_orders").format(
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/child/card.py` & `pyroostermoney-0.3.0/pyroostermoney/child/card.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Rooster Money card type."""
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-arguments
 
 from pyroostermoney.api import RoosterSession
 from pyroostermoney.const import URLS
+from pyroostermoney.events import EventSource, EventType
 
 class Card:
     """A card."""
 
     def __init__(self,
                  masked_card_number: str,
                  expiry_date: str,
@@ -15,55 +16,80 @@
                  image: str,
                  title: str,
                  description: str,
                  category: str,
                  status: str,
                  user_id: str,
                  session: RoosterSession) -> None:
+        self._card_options = {}
+        self._session = session
         self.masked_card_number = masked_card_number
         self.expiry_date = expiry_date
         self.name = name
         self.image = image
         self.title = title
         self.description = description
         self.category = category
         self.status = status
-        self._session = session
         self.user_id = user_id
         self.pin = None
+        self.card_id = None
+        self.contactless_limit = None
+        self.contactless_count = None
+        self.spend_limit = None
+        self.total_spend = None
 
     async def init_card_pin(self) -> None:
         """initializes the card pin."""
         # first we need to get the family cards
-        response = await self._session.request_handler(
-            url=URLS.get("get_family_account_cards")
-        )
-
-        if response["status"] == 200:
-            # get the card for the current user_id
-            for card in response["response"]:
-                if card["childId"] == self.user_id:
-                    response = card
-                    break
-
+        await self.update_family_card_entry()
         # if status is still in response, we didn't get a card
-        if "status" in response:
+        if "status" in self._card_options:
             raise ValueError(f"No card found for {self.user_id}")
 
         response = await self._session.request_handler(
             url=URLS.get("get_child_card_pin").format(
                 user_id=self.user_id,
-                card_id=response["cardId"]
+                card_id=self.card_id
             ),
             add_security_token=True
         )
 
         response: dict = response["response"]
         self.pin = response.get("pin", None)
 
+    async def update_family_card_entry(self):
+        """Requests an update for the internal card entry"""
+        response = await self._session.request_handler(
+            url=URLS.get("get_family_account_cards")
+        )
+
+        if response["status"] == 200:
+            # get the card for the current user_id
+            for card in response["response"]:
+                if card["childId"] == self.user_id:
+                    response = card
+                    break
+
+        self._card_options = response
+        self.card_id = response.get("cardId", None)
+        self.contactless_limit = response.get("sca", {}).get("countLimit", 5)
+        previous_count = self.contactless_count
+        self.contactless_count = response.get("sca", {}).get("count", 0)
+        self.spend_limit = response.get("sca", {}).get("spendLimit", {}).get("amount", 135)/100
+        self.total_spend = response.get("sca", {}).get("totalSpend", {}).get("amount", 135)/100
+        # raise an event if the contactless limit is reached
+        if (self.contactless_count is self.contactless_limit) and (
+            self.contactless_count is not previous_count):
+
+            self._session.events.fire_event(EventSource.CARD, EventType.UPDATED, {
+                "card_id": self.card_id,
+                "card_event": "CONTACTLESS_LIMIT"
+            })
+
     @staticmethod
     def parse_response(raw: dict, user_id: str, session: RoosterSession) -> 'Card':
         """RESPONSE PARSER"""
         return Card(
             masked_card_number = raw["image"]["maskedPan"],
             expiry_date = raw["image"]["expDate"],
             name = raw["name"],
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/child/jobs.py` & `pyroostermoney-0.3.0/pyroostermoney/child/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Job type."""
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-arguments
 from datetime import datetime
-from enum import Enum
+from enum import Enum, IntEnum
 
 from pyroostermoney.api import RoosterSession
 from pyroostermoney.const import CURRENCY, URLS
 
 class JobScheduleTypes(Enum):
     """Job schedule types."""
     REPEATING = 2
     ANYTIME = 1
     UNKNOWN = -1
 
-class JobTime(Enum):
+class JobTime(IntEnum):
     """Job times."""
     MORNING = 12
     AFTERNOON = 17
     EVENING = 22
     ANYTIME = 23
 
 class JobState(Enum):
@@ -134,15 +134,15 @@
             raw_response=raw_response["response"]
 
         output: list[Job] = []
 
         for state in raw_response:
             for job in raw_response.get(state, []):
                 output.append(Job.from_dict(job, session))
-        return output
+        return sorted(output, key=lambda job: (job.due_date, job.time_of_day), reverse=True)
 
     async def job_action(self, action: JobActions, message: str = ""):
         """Performs the given action on a scheduled job."""
         if self.scheduled_job_id is None:
             raise NotImplementedError("This function is only available on scheduled jobs.")
 
         await self._session.request_handler(
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/child/money_pot.py` & `pyroostermoney-0.3.0/pyroostermoney/child/money_pot.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/pyroostermoney/child/standing_order.py` & `pyroostermoney-0.3.0/pyroostermoney/child/standing_order.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/pyroostermoney/child/transaction.py` & `pyroostermoney-0.3.0/pyroostermoney/child/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,20 +35,22 @@
         self.message = message
         self.resource_image = resource_image
         self.transaction_timestamp = transaction_timestamp
         self.source = source
         self.transaction_type = transaction_type
         self.user_id = user_id
         self.currency = currency
+        self.declined = self.transaction_type == "CARD_DECLINE"
+        self.declined_reason = []
 
     @staticmethod
     def from_dict(obj: dict) -> 'Transaction':
         """Converts a JSON response to a Transaction type"""
 
-        return Transaction(
+        transaction = Transaction(
             action_user=obj.get("actionUserId"),
             amount=obj.get("amount"),
             new_balance=obj.get("balance"),
             currency=obj.get("currency"),
             description=obj.get("description"),
             extended_description=obj.get("descriptionExtension"),
             guardian_profile_image=obj.get("guardianProfileImage"),
@@ -56,14 +58,17 @@
             message=obj.get("message"),
             resource_image=obj.get("resourceImageURL"),
             transaction_timestamp=obj.get("time"),
             source=obj.get("transactionSource"),
             transaction_type=obj.get("type"),
             user_id=obj.get("userId")
         )
+        if transaction.declined:
+            transaction.declined_reason = obj.get("declines")
+        return transaction
 
     @staticmethod
     def parse_response(obj: list) -> list['Transaction']:
         """Parses the raw response"""
         output = []
         for action in obj:
             output.append(Transaction.from_dict(action))
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/const.py` & `pyroostermoney-0.3.0/pyroostermoney/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # pylint: disable=line-too-long
 """Static Rooster Money variables"""
 
-VERSION="0.2.5"
+VERSION="0.3.0"
 BASE_URL="https://api.rooster.money"
 OAUTH_TOKEN_URL="https://auth.rooster.money/oidc/token"
 LANGUAGE="en-GB"
 COUNTRY="gb"
 CURRENCY="GBP"
 TIMEZONE_ID=60
 TIMEZONE="GMT+01:00"
 DEFAULT_PRECISION=2
 DEFAULT_BANK_NAME="Rooster Money"
 DEFAULT_BANK_TYPE="Business"
 DEFAULT_JOB_IMAGE_URL="https://images.roostermoney.com/static/default_job_icon.png"
-MOBILE_APP_VERSION="10.3.1"
+MOBILE_APP_VERSION="10.3.2"
 
 SAVINGS_POT_ID="SAVE_POT"
 SPEND_POT_ID="SPEND_POT"
 GIVE_POT_ID="GIVE_POT"
 GOAL_POT_ID="GOAL_POT"
 
+CHILD_MAX_TRANSACTION_COUNT=15 # maximum count for get_spend_history
+
 URLS = {
     "login": "api/v1/parent",
     "get_account_info": "api/parent",
     "get_child": "api/parent/child/{user_id}",
     "get_child_allowance_periods": "api/parent/child/{user_id}/allowance-periods",
     "get_top_up_methods": "api/parent/acquirer/topup/methods?currency={currency}",
     "get_available_cards": "api/parent/acquirer/cards",
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney/exceptions.py` & `pyroostermoney-0.3.0/pyroostermoney/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/pyroostermoney/family_account.py` & `pyroostermoney-0.3.0/pyroostermoney/family_account.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/pyroostermoney/master_jobs.py` & `pyroostermoney-0.3.0/pyroostermoney/master_jobs.py`

 * *Files identical despite different names*

### Comparing `pyroostermoney-0.2.5/pyroostermoney/roostermoney.py` & `pyroostermoney-0.3.0/pyroostermoney/roostermoney.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,22 +15,18 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 class RoosterMoney(RoosterSession):
     """The RoosterMoney module."""
 
     def __init__(self,
-                 username: str,
-                 password: str,
                  update_interval: int=30,
                  use_updater: bool=False,
                  remove_card_information = False) -> None:
         super().__init__(
-            username=username,
-            password=password,
             use_updater=use_updater,
             update_interval=update_interval
         )
         self.account_info = None
         self.children: list[ChildAccount] = []
         self.master_job_list: list[Job] = []
         self.master_jobs: MasterJobs = None
@@ -42,23 +38,33 @@
         self._init = True
 
     def __del__(self):
         if self.use_updater:
             self._updater.cancel()
             self._updater = None
 
-    async def async_login(self):
-        await super().async_login()
+    @classmethod
+    async def create(cls,
+                 username: str,
+                 password: str,
+                 update_interval: int=30,
+                 remove_card_information = False):
+        """Starts a online session with Rooster Money"""
+        self = cls(update_interval=update_interval,
+                          use_updater=True,
+                          remove_card_information=remove_card_information)
+        await self._session_start(username, password)
         await self.get_family_account()
         self.master_jobs = MasterJobs(self)
         await self.update()
         if self.use_updater:
             _LOGGER.debug("Using auto updater for RoosterMoney")
             self._updater = asyncio.create_task(self._update_scheduler())
         self._init = False
+        return self
 
     async def _update_scheduler(self):
         """Automatic updater"""
         while True:
             next_time = datetime.now() + timedelta(seconds=self.update_interval)
             while datetime.now() < next_time:
                 await asyncio.sleep(1)
@@ -66,36 +72,38 @@
 
     async def update(self):
         """Perform an update of all root types"""
         if self._update_lock.locked():
             return True
 
         async with self._update_lock:
-            await self.get_children()
+            await self._update_children()
             await self.master_jobs.update()
             self.master_job_list = self.master_jobs.jobs
-            for child in self.children:
-                await child.update()
             await self.family_account.update()
 
-    async def get_children(self) -> list[ChildAccount]:
-        """Returns a list of available children."""
+    async def _update_children(self):
+        """Updates the list of available children."""
         account_info = await self.get_account_info()
         children = account_info["children"]
         for child in children:
             if child.get("userId") not in self._discovered_children:
-                child = ChildAccount(child, self, self._remove_card_information)
-                await child.perform_init() # calling this will init some extra props.
+                child = await ChildAccount.create(child.get("userId"),
+                                                self,
+                                                self._remove_card_information)
                 self._discovered_children.append(child.user_id)
                 self.children.append(child)
                 self.events.fire_event(EventSource.CHILD, EventType.CREATED, {
                     "user_id": child.user_id
                 })
         _LOGGER.debug(self._discovered_children)
         self._cleanup()
+
+    def get_children(self) -> list[ChildAccount]:
+        """Returns a list of available children (compatibility only)"""
         return self.children
 
     def _cleanup(self) -> None:
         """Removes data that no longer exists from the updater."""
         for i in range(len(self.children)):
             child_id = self.children[i-1].user_id
             if child_id not in self._discovered_children:
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney.egg-info/PKG-INFO` & `pyroostermoney-0.3.0/pyroostermoney.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroostermoney
-Version: 0.2.5
+Version: 0.3.0
 Summary: A RoosterMoney integration for Python.
 Home-page: https://github.com/pantherale0/pyroostermoney
 Author: pantherale0
 Author-email: support@system32.uk
 License: MIT
 Project-URL: Bug Tracker, https://github.com/pantherale0/pyroostermoney/issues
 Project-URL: Changelog, https://github.com/pantherale0/pyroostermoney/releases
```

### Comparing `pyroostermoney-0.2.5/pyroostermoney.egg-info/SOURCES.txt` & `pyroostermoney-0.3.0/pyroostermoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

