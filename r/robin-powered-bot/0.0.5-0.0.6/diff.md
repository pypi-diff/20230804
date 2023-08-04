# Comparing `tmp/robin-powered-bot-0.0.5.tar.gz` & `tmp/robin-powered-bot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robin-powered-bot-0.0.5.tar", last modified: Fri Jan  6 11:30:23 2023, max compression
+gzip compressed data, was "robin-powered-bot-0.0.6.tar", last modified: Fri Aug  4 14:33:13 2023, max compression
```

## Comparing `robin-powered-bot-0.0.5.tar` & `robin-powered-bot-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 11:30:23.290002 robin-powered-bot-0.0.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2581 2023-01-06 11:30:23.290002 robin-powered-bot-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2174 2023-01-06 09:48:14.000000 robin-powered-bot-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 11:30:23.290002 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2581 2023-01-06 11:30:23.000000 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-01-06 11:30:23.000000 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 11:30:23.000000 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-06 11:30:23.000000 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2023-01-06 11:30:23.000000 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-01-06 11:30:23.000000 robin-powered-bot-0.0.5/robin_powered_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 11:30:23.290002 robin-powered-bot-0.0.5/robot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/robot/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4753 2023-01-06 09:35:41.000000 robin-powered-bot-0.0.5/robot/reservations.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/robot/robin.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-01-06 11:16:40.000000 robin-powered-bot-0.0.5/robot/user.py
--rw-r--r--   0 root         (0) root         (0)       95 2023-01-06 11:30:23.300002 robin-powered-bot-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      724 2023-01-06 09:46:53.000000 robin-powered-bot-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-06 11:30:23.290002 robin-powered-bot-0.0.5/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6575 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/tests/constants.py
--rw-r--r--   0 root         (0) root         (0)     5998 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/tests/reservantions_test.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/tests/robin_test.py
--rw-r--r--   0 root         (0) root         (0)      673 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.5/tests/user_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 14:33:13.900000 robin-powered-bot-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-08-04 14:33:13.900000 robin-powered-bot-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2174 2023-01-06 09:48:14.000000 robin-powered-bot-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 14:33:13.900000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2581 2023-08-04 14:33:13.000000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-08-04 14:33:13.000000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 14:33:13.000000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 14:33:13.000000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-04 14:33:13.000000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-04 14:33:13.000000 robin-powered-bot-0.0.6/robin_powered_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 14:33:13.900000 robin-powered-bot-0.0.6/robot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.6/robot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-08-04 14:11:27.000000 robin-powered-bot-0.0.6/robot/reservations.py
+-rw-r--r--   0 root         (0) root         (0)     2401 2023-08-04 14:23:54.000000 robin-powered-bot-0.0.6/robot/robin.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-01-06 11:16:40.000000 robin-powered-bot-0.0.6/robot/user.py
+-rw-r--r--   0 root         (0) root         (0)       95 2023-08-04 14:33:13.900000 robin-powered-bot-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      724 2023-08-04 13:53:30.000000 robin-powered-bot-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 14:33:13.900000 robin-powered-bot-0.0.6/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.6/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7993 2023-08-04 14:22:17.000000 robin-powered-bot-0.0.6/tests/constants.py
+-rw-r--r--   0 root         (0) root         (0)     5998 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.6/tests/reservantions_test.py
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-08-04 14:23:25.000000 robin-powered-bot-0.0.6/tests/robin_test.py
+-rw-r--r--   0 root         (0) root         (0)      673 2023-01-06 08:51:44.000000 robin-powered-bot-0.0.6/tests/user_test.py
```

### Comparing `robin-powered-bot-0.0.5/LICENSE` & `robin-powered-bot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `robin-powered-bot-0.0.5/PKG-INFO` & `robin-powered-bot-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-powered-bot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Provides a set of utilities to simplify communication with robin-powered API and more easily automate bookings.
 Home-page: https://github.com/donatobarone/robin-powered-bot
 Author: Donato Barone
 Author-email: eng.donato.barone@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `robin-powered-bot-0.0.5/README.md` & `robin-powered-bot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `robin-powered-bot-0.0.5/robin_powered_bot.egg-info/PKG-INFO` & `robin-powered-bot-0.0.6/robin_powered_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-powered-bot
-Version: 0.0.5
+Version: 0.0.6
 Summary: Provides a set of utilities to simplify communication with robin-powered API and more easily automate bookings.
 Home-page: https://github.com/donatobarone/robin-powered-bot
 Author: Donato Barone
 Author-email: eng.donato.barone@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `robin-powered-bot-0.0.5/robot/reservations.py` & `robin-powered-bot-0.0.6/robot/reservations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import requests
 from datetime import datetime, timedelta
 from typing import List
 from robot.user import UserInfo
 
 
+class AlreadyCheckedInError(Exception):
+    pass
+
+
 class Reservation:
 
     LIST_RESERVATIONS_URL_TEMPLATE = "https://api.robinpowered.com/v1.0/reservations/seats?before={}&after={}&seat_ids={}"
     SET_RESERVATION_URL_TEMPLATE = "https://api.robinpowered.com/v1.0/seats/{}/reservations"
     CHECKIN_URL_TEMPLATE = "https://api.robinpowered.com/v1.0/reservations/seats/{}/confirmation"
     EMPTY_RESERVATION_ID = "-1"
 
@@ -67,15 +71,15 @@
         reservations = response.json()['data']
         if len(reservations) == 0:
             return self.EMPTY_RESERVATION_ID
         if len(reservations) > 1:
             raise Exception("should only contain 1 reservation")
         reservation = reservations[0]
         if reservation['confirmation'] is not None:
-            return Exception("already checked in")
+            raise AlreadyCheckedInError("desk is already checked in")
         return reservation['id']
 
     def _reserve(self) -> str:
         url, body = self.build_reserve_request(self._reservation_date_start, self._reservation_date_end,
                                                self._user_info.seat_id, self._user_info.reserver_id, self._user_info.email, self._user_info.timezone)
         response = requests.post(
             url, json=body, headers=self._headers, verify=False)
```

### Comparing `robin-powered-bot-0.0.5/robot/robin.py` & `robin-powered-bot-0.0.6/robot/robin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime, timedelta
 from typing import Dict, List
 
-from robot.reservations import Reservation
+from robot.reservations import AlreadyCheckedInError, Reservation
 
 
 class Robin:
     def __init__(self, users_info: List):
         self.users_info = users_info
 
     def daterange(self, start_date, end_date):
@@ -37,19 +37,23 @@
                 results[reserver_id][current.strftime("%Y-%m-%d")] = True
 
         return results
 
     def check_in(self, current: datetime) -> Dict:
         results = {}
         for user_info in self.users_info:
-            _, reserver_id = user_info.seat_id, user_info.reserver_id
-            reservation = Reservation(user_info, current)
-            reservation_id = reservation._get_id()
-            if "-1" == reservation_id:
-                print(f"no reservation to confirm for {reserver_id}")
-                continue
-
-            reservation._check_in(reservation_id)
-            print(f"check in successful for {reservation_id}")
-            results[reserver_id] = True
+            try:
+                _, reserver_id = user_info.seat_id, user_info.reserver_id
+                reservation = Reservation(user_info, current)
+                reservation_id = reservation._get_id()
+                if "-1" == reservation_id:
+                    print(f"no reservation to confirm for {reserver_id}")
+                    continue
 
+                reservation._check_in(reservation_id)
+                print(f"check in successful for {reservation_id}")
+                results[reserver_id] = True
+            except AlreadyCheckedInError as e:
+                print(f"error whilst checking in: {e}")                
+                results[reserver_id] = False
+                pass
         return results
```

### Comparing `robin-powered-bot-0.0.5/robot/user.py` & `robin-powered-bot-0.0.6/robot/user.py`

 * *Files identical despite different names*

### Comparing `robin-powered-bot-0.0.5/setup.py` & `robin-powered-bot-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='robin-powered-bot',
-    version='0.0.5',
+    version='0.0.6',
     description='Provides a set of utilities to simplify communication with robin-powered API and more easily automate bookings.',
     url='https://github.com/donatobarone/robin-powered-bot',
     author='Donato Barone',
     author_email='eng.donato.barone@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

### Comparing `robin-powered-bot-0.0.5/tests/constants.py` & `robin-powered-bot-0.0.6/tests/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,14 +80,66 @@
     "paging": {
         "page": 1,
         "per_page": 10,
         "has_next_page": False
     }
 }
 
+RESERVATION_CHECKED_IN_BODY = {
+    "meta": {
+        "status_code": 200,
+        "status": "OK",
+        "message": "",
+        "more_info": {},
+        "errors": []
+    },
+    "data": [{
+        "id": "2498667793369531480",
+        "group_seat_reservation_id": None,
+        "seat_id": 196962,
+        "reserver_id": 619521,
+        "type": "hoteled",
+        "title": None,
+        "start": {
+            "date_time": "2022-08-22T11:00:00+0100",
+            "time_zone": "Etc/UTC"
+        },
+        "end": {
+            "date_time": "2022-08-22T19:00:00+0100",
+            "time_zone": "Etc/UTC"
+        },
+        "recurrence": None,
+        "series_id": None,
+        "recurrence_id": None,
+        "created_at": "2023-07-22T12:06:52+0000",
+        "updated_at": "2023-08-04T13:00:49+0000",
+        "reservee": {
+            "email": "dbarone@factset.com",
+            "user_id": 619521,
+            "visitor_id": None,
+            "participation_status": "accepted"
+        },
+        "confirmation": {
+            "seat_reservation_id": "2498667793369531480",
+            "device_id": None,
+            "user_id": 619521,
+            "confirmed_at": {
+                "date": "2023-08-04 13:00:49.000000",
+                "timezone_type": 3,
+                "timezone": "UTC"
+            }
+        }
+    }],
+    "paging": {
+        "page": 1,
+        "per_page": 10,
+        "has_next_page": False
+    }
+}
+
 EMPTY_JSON_RESPONSE = {
     "meta": {
         "status_code": 200,
         "status": "OK",
         "message": "",
         "more_info": {},
         "errors": []
@@ -112,14 +164,16 @@
     },
     "reservee": {
         "email": "dbarone@factset.com"
     },
     "reserver_id": 619521
 }
 
+
+
 SUCCESSFUL_RESERVATION = {
     "meta": {
         "status_code": 200,
         "status": "OK",
         "message": "",
         "more_info": {},
         "errors": []
@@ -244,7 +298,8 @@
         "confirmed_at": {
             "date": "2022-08-26 15:19:16.111562",
             "timezone_type": 3,
             "timezone": "UTC"
         }
     }
 }
+
```

### Comparing `robin-powered-bot-0.0.5/tests/reservantions_test.py` & `robin-powered-bot-0.0.6/tests/reservantions_test.py`

 * *Files identical despite different names*

### Comparing `robin-powered-bot-0.0.5/tests/robin_test.py` & `robin-powered-bot-0.0.6/tests/robin_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pook
 
 from robot.reservations import Reservation
 from robot.robin import Robin
 from robot.user import UserInfo
 from tests.constants import (DURATION, EMPTY_JSON_RESPONSE, JSON_RESPONSE,
                              START_TIME, SUCCESSFUL_CHECK_IN,
-                             SUCCESSFUL_RESERVATION)
+                             SUCCESSFUL_RESERVATION, RESERVATION_CHECKED_IN_BODY)
 
 
 @pook.on
 def test_robin_reservation():
     users_info = [UserInfo("dbarone@factset.com", START_TIME, DURATION, 111, 619521, "Etc/UTC")]
     r = Robin(users_info)
     pook.get(Reservation.build_list_reservations_url(datetime(2022, 9, 22, 11), datetime(2022, 9, 22, 19), 111),
@@ -41,7 +41,18 @@
              reply=200, response_json=EMPTY_JSON_RESPONSE)
     url, body = Reservation.build_checkin_request(
         1, "2254519933545219475")
     pook.put(url, json=body, reply=200,
              response_json=SUCCESSFUL_CHECK_IN)
     results = r.check_in(datetime(2022, 9, 22))
     assert results == {1: True}
+
+
+@pook.on
+def test_already_checkedin_reservation():
+
+    users_info = [UserInfo("dbarone@factset.com", START_TIME, DURATION, 111, 1, "Etc/UTC")]
+    r = Robin(users_info)
+    pook.get(Reservation.build_list_reservations_url(datetime(2022, 9, 22, 11), datetime(2022, 9, 22, 19), 111),
+             reply=200, response_json=RESERVATION_CHECKED_IN_BODY)
+    results = r.check_in(datetime(2022, 9, 22))
+    assert results == {1: False}
```

### Comparing `robin-powered-bot-0.0.5/tests/user_test.py` & `robin-powered-bot-0.0.6/tests/user_test.py`

 * *Files identical despite different names*

