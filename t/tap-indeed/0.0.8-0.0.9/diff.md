# Comparing `tmp/tap-indeed-0.0.8.tar.gz` & `tmp/tap-indeed-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-indeed-0.0.8.tar", max compression
+gzip compressed data, was "tap-indeed-0.0.9.tar", max compression
```

## Comparing `tap-indeed-0.0.8.tar` & `tap-indeed-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-10-19 20:15:12.024821 tap-indeed-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-25 16:14:07.372139 tap-indeed-0.0.8/tap_indeedsponsoredjobs/__init__.py
--rw-r--r--   0        0        0     8823 2022-10-19 20:14:05.321209 tap-indeed-0.0.8/tap_indeedsponsoredjobs/auth.py
--rw-r--r--   0        0        0    12293 2022-10-19 15:49:50.472052 tap-indeed-0.0.8/tap_indeedsponsoredjobs/client.py
--rw-r--r--   0        0        0     6625 2022-10-01 15:31:21.224115 tap-indeed-0.0.8/tap_indeedsponsoredjobs/streams.py
--rw-r--r--   0        0        0     1528 2022-10-01 15:30:30.292255 tap-indeed-0.0.8/tap_indeedsponsoredjobs/tap.py
--rw-r--r--   0        0        0       46 2022-09-25 16:14:07.372139 tap-indeed-0.0.8/tap_indeedsponsoredjobs/tests/__init__.py
--rw-r--r--   0        0        0     1861 2022-10-19 18:23:07.924523 tap-indeed-0.0.8/tap_indeedsponsoredjobs/tests/test_core.py
--rw-r--r--   0        0        0      980 2022-10-19 20:16:00.265269 tap-indeed-0.0.8/setup.py
--rw-r--r--   0        0        0      713 2022-10-19 20:16:00.265425 tap-indeed-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-11-18 04:39:56.946177 tap-indeed-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-25 16:14:07.372139 tap-indeed-0.0.9/tap_indeedsponsoredjobs/__init__.py
+-rw-r--r--   0        0        0     8823 2022-11-18 04:38:14.578427 tap-indeed-0.0.9/tap_indeedsponsoredjobs/auth.py
+-rw-r--r--   0        0        0    12293 2022-11-18 04:38:14.578427 tap-indeed-0.0.9/tap_indeedsponsoredjobs/client.py
+-rw-r--r--   0        0        0     6726 2022-11-18 04:39:07.498294 tap-indeed-0.0.9/tap_indeedsponsoredjobs/streams.py
+-rw-r--r--   0        0        0     1528 2022-11-18 04:38:14.578427 tap-indeed-0.0.9/tap_indeedsponsoredjobs/tap.py
+-rw-r--r--   0        0        0       46 2022-09-25 16:14:07.372139 tap-indeed-0.0.9/tap_indeedsponsoredjobs/tests/__init__.py
+-rw-r--r--   0        0        0     1861 2022-11-18 04:38:14.578427 tap-indeed-0.0.9/tap_indeedsponsoredjobs/tests/test_core.py
+-rw-r--r--   0        0        0      980 2022-11-18 04:41:01.051396 tap-indeed-0.0.9/setup.py
+-rw-r--r--   0        0        0      713 2022-11-18 04:41:01.051561 tap-indeed-0.0.9/PKG-INFO
```

### Comparing `tap-indeed-0.0.8/pyproject.toml` & `tap-indeed-0.0.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-indeed"
-version = "0.0.8"
+version = "0.0.9"
 description = "`tap-indeed` is a Singer tap for IndeedSponsoredJobs, built with the Meltano SDK for Singer Taps."
 authors = ["AutoIDM"]
 keywords = [
     "ELT",
     "IndeedSponsoredJobs",
     "tap-indeed",
     "Indeed",
```

### Comparing `tap-indeed-0.0.8/tap_indeedsponsoredjobs/auth.py` & `tap-indeed-0.0.9/tap_indeedsponsoredjobs/auth.py`

 * *Files identical despite different names*

### Comparing `tap-indeed-0.0.8/tap_indeedsponsoredjobs/client.py` & `tap-indeed-0.0.9/tap_indeedsponsoredjobs/client.py`

 * *Files identical despite different names*

### Comparing `tap-indeed-0.0.8/tap_indeedsponsoredjobs/streams.py` & `tap-indeed-0.0.9/tap_indeedsponsoredjobs/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,20 +81,21 @@
 
 class CampaignPerformanceStats(IndeedSponsoredJobsStream):
     """Campaign Performance per Campaign"""
     name = "campaign_performance_stats"
     path = "/v1/campaigns/{_sdc_campaign_id}/stats"
     primary_keys = ["Id", "Date"]
     records_jsonpath = "$.['data']['entries'][*]"
-    replication_key = None
+    replication_key = "Date"
+    is_sorted = False
     parent_stream_type = Campaigns
     schema = th.PropertiesList(
             th.Property("Name", th.StringType),
             th.Property("Id", th.StringType),
-            th.Property("Date", th.StringType),
+            th.Property("Date", th.DateType),
             th.Property("Clicks", th.IntegerType),
             th.Property("Impressions", th.IntegerType),
             th.Property("Conversions", th.IntegerType),
             th.Property("CurrencyCode", th.StringType),
             th.Property("Cost", th.NumberType),
             th.Property("OrganicClicks", th.IntegerType),
             th.Property("OrganicImpressions", th.IntegerType),
@@ -111,15 +112,17 @@
         #TODO call super
         #if next_page_token:
         #    params["page"] = next_page_token
         #if self.replication_key:
         #    params["sort"] = "asc"
         #    params["order_by"] = self.replication_key
         params["perPage"]=1000000000
-        params["startDate"]=self.config["start_date"]
+        #params["startDate"]=self.config["start_date"]
+        params["startDate"]=self.get_starting_replication_key_value(context)
+
         return params
 
 class CampaignBudget(IndeedSponsoredJobsStream):
     """Campaign Budget per Campaign"""
     name = "campaign_budget"
     path = "/v1/campaigns/{_sdc_campaign_id}/budget"
     primary_keys = ["_sdc_campaign_id"]
```

### Comparing `tap-indeed-0.0.8/tap_indeedsponsoredjobs/tap.py` & `tap-indeed-0.0.9/tap_indeedsponsoredjobs/tap.py`

 * *Files identical despite different names*

### Comparing `tap-indeed-0.0.8/tap_indeedsponsoredjobs/tests/test_core.py` & `tap-indeed-0.0.9/tap_indeedsponsoredjobs/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap-indeed-0.0.8/setup.py` & `tap-indeed-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 entry_points = \
 {'console_scripts': ['tap-indeedsponsoredjobs = '
                      'tap_indeedsponsoredjobs.tap:TapIndeedSponsoredJobs.cli']}
 
 setup_kwargs = {
     'name': 'tap-indeed',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '`tap-indeed` is a Singer tap for IndeedSponsoredJobs, built with the Meltano SDK for Singer Taps.',
     'long_description': None,
     'author': 'AutoIDM',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `tap-indeed-0.0.8/PKG-INFO` & `tap-indeed-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-indeed
-Version: 0.0.8
+Version: 0.0.9
 Summary: `tap-indeed` is a Singer tap for IndeedSponsoredJobs, built with the Meltano SDK for Singer Taps.
 License: Apache 2.0
 Keywords: ELT,IndeedSponsoredJobs,tap-indeed,Indeed,singer-sdk,meltano
 Author: AutoIDM
 Requires-Python: >=3.7.1,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

