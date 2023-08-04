# Comparing `tmp/pyGuardPoint-0.9.9.tar.gz` & `tmp/pyGuardPoint-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGuardPoint-0.9.9.tar", last modified: Wed Aug  2 09:22:37 2023, max compression
+gzip compressed data, was "pyGuardPoint-1.0.0.tar", last modified: Fri Aug  4 12:40:39 2023, max compression
```

## Comparing `pyGuardPoint-0.9.9.tar` & `pyGuardPoint-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 09:22:37.284077 pyGuardPoint-0.9.9/
--rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-0.9.9/LICENSE.txt
--rw-rw-rw-   0        0        0     6116 2023-08-02 09:22:37.283087 pyGuardPoint-0.9.9/PKG-INFO
--rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-0.9.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-02 09:22:37.276080 pyGuardPoint-0.9.9/pyGuardPoint/
--rw-rw-rw-   0        0        0      266 2023-04-20 12:58:39.000000 pyGuardPoint-0.9.9/pyGuardPoint/__init__.py
--rw-rw-rw-   0        0        0      997 2023-03-03 10:58:18.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_areas.py
--rw-rw-rw-   0        0        0    11195 2023-04-20 13:33:25.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholders.py
--rw-rw-rw-   0        0        0     1083 2023-04-20 13:02:16.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholdertypes.py
--rw-rw-rw-   0        0        0     6687 2023-04-05 13:08:15.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cards.py
--rw-rw-rw-   0        0        0     1170 2023-03-16 16:56:01.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_customizedfields.py
--rw-rw-rw-   0        0        0     1195 2023-05-12 10:57:02.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_personaldetails.py
--rw-rw-rw-   0        0        0     2462 2023-03-17 15:44:40.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_scheduledmags.py
--rw-rw-rw-   0        0        0     1314 2023-03-17 12:07:11.000000 pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_securitygroups.py
--rw-rw-rw-   0        0        0     5584 2023-08-02 09:21:03.000000 pyGuardPoint-0.9.9/pyGuardPoint/_odata_filter.py
--rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-0.9.9/pyGuardPoint/_str_match_algo.py
--rw-rw-rw-   0        0        0     2915 2023-07-26 07:31:58.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint.py
--rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_async.py
--rw-rw-rw-   0        0        0    10663 2023-07-31 14:11:21.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_connection.py
--rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_dataclasses.py
--rw-rw-rw-   0        0        0       49 2023-03-21 15:31:43.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_error.py
--rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 09:22:37.282077 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/
--rw-rw-rw-   0        0        0     6116 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      861 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       47 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-08-02 09:22:37.000000 pyGuardPoint-0.9.9/pyGuardPoint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 09:22:37.284077 pyGuardPoint-0.9.9/setup.cfg
--rw-rw-rw-   0        0        0      565 2023-08-02 09:21:40.000000 pyGuardPoint-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 13:07:38.000000 pyGuardPoint-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     6116 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5857 2023-07-26 10:18:05.000000 pyGuardPoint-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-04 12:40:39.103820 pyGuardPoint-1.0.0/pyGuardPoint/
+-rw-rw-rw-   0        0        0      290 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-08-04 12:11:20.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_areas.py
+-rw-rw-rw-   0        0        0    12153 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholders.py
+-rw-rw-rw-   0        0        0     1415 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholdertypes.py
+-rw-rw-rw-   0        0        0     6900 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cards.py
+-rw-rw-rw-   0        0        0     1385 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_customizedfields.py
+-rw-rw-rw-   0        0        0     1408 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_personaldetails.py
+-rw-rw-rw-   0        0        0     2648 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_scheduledmags.py
+-rw-rw-rw-   0        0        0     1500 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_securitygroups.py
+-rw-rw-rw-   0        0        0     5584 2023-08-02 09:21:03.000000 pyGuardPoint-1.0.0/pyGuardPoint/_odata_filter.py
+-rw-rw-rw-   0        0        0     1636 2023-03-31 09:30:04.000000 pyGuardPoint-1.0.0/pyGuardPoint/_str_match_algo.py
+-rw-rw-rw-   0        0        0     2988 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint.py
+-rw-rw-rw-   0        0        0     4058 2023-04-05 09:36:31.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_async.py
+-rw-rw-rw-   0        0        0    10663 2023-07-31 14:11:21.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_connection.py
+-rw-rw-rw-   0        0        0    17658 2023-05-12 10:58:18.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_dataclasses.py
+-rw-rw-rw-   0        0        0      105 2023-08-04 12:11:20.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_error.py
+-rw-rw-rw-   0        0        0     3140 2023-05-04 10:22:18.000000 pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/
+-rw-rw-rw-   0        0        0     6116 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-30 14:14:07.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       47 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-08-04 12:40:39.000000 pyGuardPoint-1.0.0/pyGuardPoint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 12:40:39.113928 pyGuardPoint-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      565 2023-08-04 12:40:14.000000 pyGuardPoint-1.0.0/setup.py
```

### Comparing `pyGuardPoint-0.9.9/LICENSE.txt` & `pyGuardPoint-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/PKG-INFO` & `pyGuardPoint-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.9
+Version: 1.0.0
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.9/README.rst` & `pyGuardPoint-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_areas.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholdertypes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-from .guardpoint_dataclasses import Area
-from .guardpoint_error import GuardPointError
+from .guardpoint_dataclasses import CardholderType
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
-class AreasAPI:
-    def get_areas(self):
-        url = "/odata/API_Areas"
+class CardholderTypesAPI:
+    def get_cardholder_types(self):
+        url = "/odata/API_CardholderTypes"
         headers = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         code, json_body = self.gp_json_query("GET", headers=headers, url=url)
 
         if code != 200:
+            error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
+                    error_msg = json_body['error']
+                elif 'message' in json_body:
+                    error_msg = json_body['message']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            else:
+                raise GuardPointError(f"No body - ({code})")
 
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'value' not in json_body:
             raise GuardPointError("Badly formatted response.")
         if not isinstance(json_body['value'], list):
             raise GuardPointError("Badly formatted response.")
 
-        areas = []
+        cardholder_types = []
         for x in json_body['value']:
-            areas.append(Area(x))
-        return areas
+            cardholder_types.append(CardholderType(x))
+        return cardholder_types
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cardholders.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cardholders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 
 import validators
 from ._odata_filter import _compose_filter, _compose_select, _compose_expand
 from ._str_match_algo import fuzzy_match
 from .guardpoint_dataclasses import Cardholder, SortAlgorithm, Area
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 from .guardpoint_utils import GuardPointResponse
 
 
 class CardholdersAPI:
 
     def delete_card_holder(self, cardholder: Cardholder):
         if not validators.uuid(cardholder.uid):
@@ -84,20 +84,27 @@
 
         code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
         # Check response body is formatted correctly
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 204:  # HTTP NO_CONTENT
-            if 'error' in json_body:
-                raise GuardPointError(json_body['error'])
-            elif 'message' in json_body:
-                raise GuardPointError(json_body['message'])
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+                elif 'message' in json_body:
+                    error_msg = json_body['message']
+                else:
+                    error_msg = str(code)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
         return True
 
     def new_card_holder(self, cardholder: Cardholder, overwrite_cardholder=False):
 
         # url = "/odata/API_Cardholders/CreateFullCardholder"
         url = "/odata/API_Cardholders"
@@ -138,20 +145,30 @@
             return self._get_card_holder(new_cardholder.uid)
 
         elif code == 422:  # unprocessable Entity
             if "errorMessages" in json_body:
                 raise GuardPointError(
                     f'{json_body["errorMessages"][0]["message"]}-{json_body["errorMessages"][0]["other"]}')
         else:
-            if "errorMessages" in json_body:
-                raise GuardPointError(json_body["errorMessages"][0]["other"])
-            elif "error" in json_body:
-                raise GuardPointError(json_body["error"]['message'])
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+                elif "errorMessages" in json_body:
+                    error_msg = json_body["errorMessages"][0]["other"]
+                elif "error" in json_body:
+                    error_msg = GuardPointError(json_body["error"]['message'])
+                else:
+                    error_msg = str(code)
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
+
 
     def get_card_holder(self,
                         uid: str = None,
                         card_code: str = None):
         if card_code:
             # Part of the Cards_API
             return self.get_cardholder_by_card_code(card_code)
@@ -167,19 +184,23 @@
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
         # Check response body is formatted correctly
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 200:
+            error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
         return json_body['value'][0]['photo']
 
     def _get_card_holder(self, uid):
         if not validators.uuid(uid):
             raise ValueError(f'Malformed UID {uid}')
 
@@ -198,19 +219,23 @@
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code == 404: # Not Found
             return None
 
         if code != 200:
+            error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
         return Cardholder(json_body['value'][0])
 
     def get_card_holders(self, offset: int = 0, limit: int = 10, search_terms: str = None, areas: list = None,
                          filter_expired: bool = False, cardholder_type_name: str = None,
                          sort_algorithm: SortAlgorithm = SortAlgorithm.SERVER_DEFAULT, threshold: int = 75,
                          count: bool = False, earliest_last_pass: datetime = None,
@@ -247,19 +272,21 @@
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
         # Check response body is formatted correctly
         if json_body:
             GuardPointResponse.check_odata_body_structure(json_body)
 
         if code != 200:
-            if json_body:
+            error_msg = ""
+            if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(f"{json_body['error']} - ({code})")
-                else:
-                    raise GuardPointError(f"No error message - ({code})")
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
                 raise GuardPointError(f"No body - ({code})")
 
         if count:
             return json_body['@odata.count']
 
         cardholders = []
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_cards.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_cards.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import validators
 
 from ._odata_filter import _compose_select, _compose_filter
 from .guardpoint_dataclasses import Card, Cardholder
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class CardsAPI:
     def get_cards(self, count=False, **card_kwargs):
         # Filter arguments which have to exact match
         match_args = dict()
         for k, v in card_kwargs.items():
@@ -86,20 +86,25 @@
         }
 
         ch = card.dict(changed_only=True)
 
         code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
 
         if code != 204:  # HTTP NO_CONTENT
-            if 'error' in json_body:
-                raise GuardPointError(json_body['error'])
-            elif 'message' in json_body:
-                raise GuardPointError(json_body['message'])
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+                elif 'message' in json_body:
+                    error_msg = json_body['message']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
         return True
 
     def new_card(self, card: Card):
         url = "/odata/API_Cards"
         headers = {
             'Content-Type': 'application/json',
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_customizedfields.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_customizedfields.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import validators
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 from .guardpoint_dataclasses import CardholderCustomizedField
 
 
 class CustomizedFieldsAPI:
 
     def update_custom_fields(self, cardholder_uid: str, customFields: CardholderCustomizedField):
@@ -20,15 +20,21 @@
         }
 
         ch = customFields.dict(changed_only=True)
 
         code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
 
         if code != 204:  # HTTP NO_CONTENT
-            if 'error' in json_body:
-                raise GuardPointError(json_body['error'])
-            elif 'message' in json_body:
-                raise GuardPointError(json_body['message'])
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+                elif 'message' in json_body:
+                    error_msg = json_body['message']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
+
 
         return True
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_personaldetails.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_personaldetails.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import validators
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 from .guardpoint_dataclasses import CardholderPersonalDetail
 
 
 class PersonalDetailsAPI:
 
     def update_personal_details(self, cardholder_uid: str, personal_details: CardholderPersonalDetail):
@@ -20,15 +20,20 @@
         }
 
         ch = personal_details.dict(editable_only=True, changed_only=True)
 
         code, json_body = self.gp_json_query("PATCH", headers=headers, url=(url + url_query_params), json_body=ch)
 
         if code != 204:  # HTTP NO_CONTENT
-            if 'error' in json_body:
-                raise GuardPointError(json_body['error'])
-            elif 'message' in json_body:
-                raise GuardPointError(json_body['message'])
+            error_msg = ""
+            if isinstance(json_body, dict):
+                if 'error' in json_body:
+                    error_msg = json_body['error']
+                elif 'message' in json_body:
+                    error_msg = json_body['message']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
         return True
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_scheduledmags.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_scheduledmags.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import validators
 
 from .guardpoint_dataclasses import ScheduledMag, Cardholder
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class ScheduledMagsAPI:
 
     def get_scheduled_mags(self, cardholder: Cardholder = None):
         url = self.baseurl + "/odata/API_ScheduledMags"
         if cardholder:
@@ -14,18 +14,23 @@
             url_query_params = f"?$filter=cardholderUid%20eq%20'{cardholder.uid}'"
         else:
             url_query_params = ""
 
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
 
         if code != 200:
+            error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-            raise GuardPointError(str(code))
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            else:
+                raise GuardPointError(f"No body - ({code})")
 
         # Check response body is formatted as expected
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'value' not in json_body:
             raise GuardPointError("Badly formatted response.")
         if not isinstance(json_body['value'], list):
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_guardpoint_securitygroups.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_guardpoint_securitygroups.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from .guardpoint_dataclasses import SecurityGroup
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 
 
 class SecurityGroupsAPI:
     def get_security_groups(self):
         url = self.baseurl + "/odata/api_SecurityGroups"
         # url_query_params = "?$select=uid,name&$filter=name%20ne%20'Anytime%20Anywhere'"
         url_query_params = ""
         code, json_body = self.gp_json_query("GET", url=(url + url_query_params))
 
         if code != 200:
+            error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
-            raise GuardPointError(str(code))
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
+            else:
+                raise GuardPointError(f"No body - ({code})")
 
         # Check response body is formatted as expected
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'value' not in json_body:
             raise GuardPointError("Badly formatted response.")
         if not isinstance(json_body['value'], list):
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_odata_filter.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_odata_filter.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/_str_match_algo.py` & `pyGuardPoint-1.0.0/pyGuardPoint/_str_match_algo.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint.py` & `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from ._guardpoint_scheduledmags import ScheduledMagsAPI
 from ._guardpoint_customizedfields import CustomizedFieldsAPI
 from ._guardpoint_personaldetails import PersonalDetailsAPI
 from ._guardpoint_securitygroups import SecurityGroupsAPI
 from .guardpoint_connection import GuardPointConnection, GuardPointAuthType
 from ._guardpoint_cards import CardsAPI
 from ._guardpoint_cardholders import CardholdersAPI
-from .guardpoint_error import GuardPointError
+from .guardpoint_error import GuardPointError, GuardPointUnauthorized
 from ._guardpoint_areas import AreasAPI
 from .guardpoint_utils import url_parser
 
 log = logging.getLogger(__name__)
 
 
 class GuardPoint(GuardPointConnection, CardsAPI, CardholdersAPI, AreasAPI, SecurityGroupsAPI,
@@ -39,30 +39,29 @@
         timeout = kwargs.get('timeout', 5)
         p12_file = kwargs.get('p12_file', None)
         p12_pwd = kwargs.get('p12_pwd', "")
         super().__init__(url_components=url_components, auth=auth, user=user, pwd=pwd, key=key, token=token,
                          cert_file=certfile, key_file=keyfile, ca_file=cafile, timeout=timeout,
                          p12_file=p12_file, p12_pwd=p12_pwd)
 
-
-
-    # TODO: is this needed since count can be achieved with "$count=true&$top=0"
     def get_cardholder_count(self):
         url = self.baseurl + "/odata/GetCardholdersCount"
         code, json_body = self.gp_json_query("GET", url=url)
 
         if code != 200:
+            error_msg = ""
             if isinstance(json_body, dict):
                 if 'error' in json_body:
-                    raise GuardPointError(json_body['error'])
+                    error_msg = json_body['error']
+
+            if code == 401:
+                raise GuardPointUnauthorized(f"Unauthorized - ({error_msg})")
             else:
-                raise GuardPointError(str(code))
+                raise GuardPointError(f"No body - ({code})")
 
         # Check response body is formatted as expected
         if not isinstance(json_body, dict):
             raise GuardPointError("Badly formatted response.")
         if 'totalItems' not in json_body:
             raise GuardPointError("Badly formatted response.")
 
         return int(json_body['totalItems'])
-
-
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_async.py` & `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_async.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_connection.py` & `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_connection.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_dataclasses.py` & `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint/guardpoint_utils.py` & `pyGuardPoint-1.0.0/pyGuardPoint/guardpoint_utils.py`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint.egg-info/PKG-INFO` & `pyGuardPoint-1.0.0/pyGuardPoint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyGuardPoint
-Version: 0.9.9
+Version: 1.0.0
 Summary: Python wrapper for GuardPoint 10 Access Control System
 Author: John Owen
 Maintainer-email: sales@sensoraccess.co.uk
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 pyGuardPoint
```

### Comparing `pyGuardPoint-0.9.9/pyGuardPoint.egg-info/SOURCES.txt` & `pyGuardPoint-1.0.0/pyGuardPoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyGuardPoint-0.9.9/setup.py` & `pyGuardPoint-1.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 long_description = open('README.rst').read()
 
 setup(name="pyGuardPoint",
-      version="0.9.9",
+      version="1.0.0",
       author="John Owen",
       description="Python wrapper for GuardPoint 10 Access Control System",
       long_description_content_type='text/markdown',
       long_description=long_description,
       maintainer_email="sales@sensoraccess.co.uk",
       install_requires=['validators', 'fuzzywuzzy', 'Levenshtein', 'cryptography'],
       packages=['pyGuardPoint'],
```

