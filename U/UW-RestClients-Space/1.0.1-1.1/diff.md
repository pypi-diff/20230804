# Comparing `tmp/UW-RestClients-Space-1.0.1.tar.gz` & `tmp/UW-RestClients-Space-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-Space-1.0.1.tar", last modified: Tue Nov 16 18:48:22 2021, max compression
+gzip compressed data, was "UW-RestClients-Space-1.1.tar", last modified: Fri Dec  2 22:15:40 2022, max compression
```

## Comparing `UW-RestClients-Space-1.0.1.tar` & `UW-RestClients-Space-1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.833455 UW-RestClients-Space-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       54 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)      663 2021-11-16 18:48:22.833455 UW-RestClients-Space-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1141 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)      663 2021-11-16 18:48:22.000000 UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      582 2021-11-16 18:48:22.000000 UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-11-16 18:48:22.000000 UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2021-11-16 18:48:22.000000 UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2021-11-16 18:48:22.000000 UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-11-16 18:48:22.833455 UW-RestClients-Space-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1189 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/
--rw-r--r--   0 runner    (1001) docker     (116)        6 2021-11-16 18:48:22.000000 UW-RestClients-Space-1.0.1/uw_space/VERSION
--rw-r--r--   0 runner    (1001) docker     (116)     1926 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      427 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/dao.py
--rw-r--r--   0 runner    (1001) docker     (116)     1821 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/models.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/resources/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/resources/space/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/resources/space/file/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/resources/space/file/space/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/resources/space/file/space/v1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/resources/space/file/space/v1/facility/
--rw-r--r--   0 runner    (1001) docker     (116)     1006 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/resources/space/file/space/v1/facility/1347.json
--rw-r--r--   0 runner    (1001) docker     (116)     1334 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/resources/space/file/space/v1/facility.json_facility_code_MEB
--rw-r--r--   0 runner    (1001) docker     (116)      465 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/test.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:22.829455 UW-RestClients-Space-1.0.1/uw_space/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      607 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (116)     1124 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/tests/test_facilities.py
--rw-r--r--   0 runner    (1001) docker     (116)      401 2021-11-16 18:48:13.000000 UW-RestClients-Space-1.0.1/uw_space/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)       54 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)      641 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1141 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.429443 UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)      641 2022-12-02 22:15:40.000000 UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      582 2022-12-02 22:15:40.000000 UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-12-02 22:15:40.000000 UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       25 2022-12-02 22:15:40.000000 UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2022-12-02 22:15:40.000000 UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1189 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/uw_space/
+-rw-r--r--   0 runner    (1001) docker     (116)        4 2022-12-02 22:15:39.000000 UW-RestClients-Space-1.1/uw_space/VERSION
+-rw-r--r--   0 runner    (1001) docker     (116)     1927 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      428 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/dao.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1822 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/models.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.429443 UW-RestClients-Space-1.1/uw_space/resources/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.429443 UW-RestClients-Space-1.1/uw_space/resources/space/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.429443 UW-RestClients-Space-1.1/uw_space/resources/space/file/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.429443 UW-RestClients-Space-1.1/uw_space/resources/space/file/space/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/uw_space/resources/space/file/space/v2/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/uw_space/resources/space/file/space/v2/facility/
+-rw-r--r--   0 runner    (1001) docker     (116)     1139 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/resources/space/file/space/v2/facility/1347.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1334 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB
+-rw-r--r--   0 runner    (1001) docker     (116)      466 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/test.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:40.433443 UW-RestClients-Space-1.1/uw_space/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      571 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1125 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/tests/test_facilities.py
+-rw-r--r--   0 runner    (1001) docker     (116)      402 2022-12-02 22:15:31.000000 UW-RestClients-Space-1.1/uw_space/utils.py
```

### Comparing `UW-RestClients-Space-1.0.1/LICENSE` & `UW-RestClients-Space-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.0.1/PKG-INFO` & `UW-RestClients-Space-1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-Space
-Version: 1.0.1
+Version: 1.1
 Summary: A library for connecting to HFS services at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-space
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 
 
 See the README on `GitHub
 <https://github.com/uw-it-aca/uw-restclients-space>`_.
-
-
```

### Comparing `UW-RestClients-Space-1.0.1/README.md` & `UW-RestClients-Space-1.1/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/PKG-INFO` & `UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-Space
-Version: 1.0.1
+Version: 1.1
 Summary: A library for connecting to HFS services at the University of Washington
 Home-page: https://github.com/uw-it-aca/uw-restclients-space
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 
 
 See the README on `GitHub
 <https://github.com/uw-it-aca/uw-restclients-space>`_.
-
-
```

### Comparing `UW-RestClients-Space-1.0.1/UW_RestClients_Space.egg-info/SOURCES.txt` & `UW-RestClients-Space-1.1/UW_RestClients_Space.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 UW_RestClients_Space.egg-info/top_level.txt
 uw_space/VERSION
 uw_space/__init__.py
 uw_space/dao.py
 uw_space/models.py
 uw_space/test.py
 uw_space/utils.py
-uw_space/resources/space/file/space/v1/facility.json_facility_code_MEB
-uw_space/resources/space/file/space/v1/facility/1347.json
+uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB
+uw_space/resources/space/file/space/v2/facility/1347.json
 uw_space/tests/__init__.py
 uw_space/tests/test_dao.py
 uw_space/tests/test_facilities.py
```

### Comparing `UW-RestClients-Space-1.0.1/setup.py` & `UW-RestClients-Space-1.1/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Space-1.0.1/uw_space/__init__.py` & `UW-RestClients-Space-1.1/uw_space/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-# Copyright 2021 UW-IT, University of Washington
+# Copyright 2022 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
+
 import json
 import logging
 from restclients_core.exceptions import DataFailureException
 from uw_space.dao import SPACE_DAO
 from uw_space.models import Facility
 
-by_code_path = "/space/v1/facility.json?facility_code={}"
-by_number_path = "/space/v1/facility/{}.json"
+by_code_path = "/space/v2/facility.json?facility_code={}"
+by_number_path = "/space/v2/facility/{}.json"
 logger = logging.getLogger(__name__)
 
 
 class Facilities(object):
 
     def __init__(self):
         self.dao = SPACE_DAO()
```

### Comparing `UW-RestClients-Space-1.0.1/uw_space/models.py` & `UW-RestClients-Space-1.1/uw_space/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Copyright 2021 UW-IT, University of Washington
+# Copyright 2022 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
+
 import json
 from restclients_core import models
 from uw_space.utils import date_to_str, str_to_datetime
 
 
 class Facility(models.Model):
     code = models.CharField(max_length=16)
```

### Comparing `UW-RestClients-Space-1.0.1/uw_space/resources/space/file/space/v1/facility/1347.json` & `UW-RestClients-Space-1.1/uw_space/resources/space/file/space/v2/facility.json_facility_code_MEB`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('TotalCount', 1), ('Facilitys', [OrderedDict([('FacilityCode', 'MEB'), "*

 * *            "('FacilityType', OrderedDict([('Code', 'BLDG'), ('Description', 'Building')])), "*

 * *            "('Status', 'A'), ('AggregateFacilityNumber', '1347'), ('Site', 'SEA_MN'), ('Name', "*

 * *            "'Mechanical Engr Bldg'), ('LongName', 'Mechanical Engineering Building'), "*

 * *            "('LeasedOrOwned', 'OWNED'), ('OFMCountyCode', '17'), ('StreetAddress', None), "*

 * *            "('City', None), ('State' […]*

```diff
@@ -1,45 +1,53 @@
 {
-    "Addresses": [
+    "Current": {
+        "AggregateNumber": null,
+        "City": null,
+        "FacilityCode": "MEB",
+        "FacilityType": null,
+        "Href": "/space/v2/facility.json?facility_type=&facility_code=MEB&status=&aggregate_number=&site=&name=&long_name=&leased_or_owned=&street=&city=&state=&postal_code=&page_start=1&page_size=10",
+        "LeasedOrOwned": null,
+        "LongName": null,
+        "Name": null,
+        "PageSize": "10",
+        "PageStart": "1",
+        "PostalCode": null,
+        "Site": null,
+        "State": null,
+        "Status": null,
+        "Street": null
+    },
+    "Facilitys": [
         {
-            "CenterPoint": {
-                "Latitude": "0.0",
-                "Longitude": "0.0"
-            },
+            "AggregateFacilityNumber": "1347",
             "City": null,
-            "Code": null,
             "Country": null,
             "CountryCode2": null,
             "CountryCode3": null,
             "County": null,
+            "FacilityCode": "MEB",
+            "FacilityNumber": "1347",
+            "FacilityType": {
+                "Code": "BLDG",
+                "Description": "Building"
+            },
+            "FacilityURI": {
+                "Description": "Mechanical Engr Bldg",
+                "FacilityCode": "MEB",
+                "FacilityNumber": "1347",
+                "Href": "/space/v2/facility/1347.json"
+            },
+            "LeasedOrOwned": "OWNED",
+            "LongName": "Mechanical Engineering Building",
+            "Name": "Mechanical Engr Bldg",
+            "OFMCountyCode": "17",
             "PostalCode": null,
-            "PrimaryAddress": "Y",
+            "Site": "SEA_MN",
             "State": null,
+            "Status": "A",
             "StreetAddress": null
         }
     ],
-    "AggregateFacilityNumber": "1347",
-    "CenterPoint": {
-        "Latitude": "47.653693",
-        "Longitude": "-122.304747"
-    },
-    "ConstructionType": "M/W",
-    "FacilityCode": "MEB",
-    "FacilityNumber": "1347",
-    "FacilityType": {
-        "Code": "BLDG",
-        "Description": "Building"
-    },
-    "GrossSquareFeet": "97768",
-    "IsRegisteredHistoricSite": "N",
-    "LeasedOrOwned": "OWNED",
-    "LongName": "Mechanical Engineering Building",
-    "ModifiedDate": "3/27/2021 4:53:09 AM",
-    "Name": "Mechanical Engr Bldg",
-    "OFMCountyCode": "17",
-    "RoomCount": 252,
-    "Site": {
-        "Code": "SEA_MN",
-        "Description": "Seattle Main Campus"
-    },
-    "Status": "A"
+    "Next": null,
+    "Previous": null,
+    "TotalCount": 1
 }
```

### Comparing `UW-RestClients-Space-1.0.1/uw_space/tests/test_dao.py` & `UW-RestClients-Space-1.1/uw_space/tests/test_dao.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-# Copyright 2021 UW-IT, University of Washington
+# Copyright 2022 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
+
 from unittest import TestCase
 import mock
 from commonconf import override_settings
 from restclients_core.exceptions import DataFailureException
 from uw_space.dao import SPACE_DAO
 from uw_space.utils import fdao_space_override
 
@@ -12,9 +13,8 @@
 @fdao_space_override
 class TestSpaceDao(TestCase):
 
     def test_dao(self):
         dao = SPACE_DAO()
         self.assertEqual(dao.service_name(), "space")
         self.assertTrue(
-            dao.service_mock_paths()[0].endswith(
-                "uw-restclients-space/uw_space/resources"))
+            dao.service_mock_paths()[0].endswith("/uw_space/resources"))
```

### Comparing `UW-RestClients-Space-1.0.1/uw_space/tests/test_facilities.py` & `UW-RestClients-Space-1.1/uw_space/tests/test_facilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright 2021 UW-IT, University of Washington
+# Copyright 2022 UW-IT, University of Washington
 # SPDX-License-Identifier: Apache-2.0
 
+
 from unittest import TestCase
 from restclients_core.exceptions import DataFailureException
 from uw_space import Facilities
 from uw_space.utils import fdao_space_override
 
 data = {
     'code': 'MEB',
-    'last_updated': '2021-03-27 04:53:09',
-    'latitude': '47.653693',
-    'longitude': '-122.304747',
+    'last_updated': '2022-09-22 19:41:34',
+    'latitude': 47.6536929997,
+    'longitude': -122.304747,
     'name': 'Mechanical Engineering Building',
     'number': '1347',
     'site': 'Seattle Main Campus',
     'type': 'Building'
     }
```

