# Comparing `tmp/alibabacloud_linkcard20210520_py2-1.0.8.tar.gz` & `tmp/alibabacloud_linkcard20210520_py2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkcard20210520_py2-1.0.8.tar", last modified: Wed Apr 12 07:08:09 2023, max compression
+gzip compressed data, was "dist/alibabacloud_linkcard20210520_py2-1.0.9.tar", last modified: Wed Jun 28 06:54:03 2023, max compression
```

## Comparing `alibabacloud_linkcard20210520_py2-1.0.8.tar` & `alibabacloud_linkcard20210520_py2-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      547 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42160 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/client.py
--rw-r--r--   0 root         (0) root         (0)   238312 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2023-04-12 07:08:09.000000 alibabacloud_linkcard20210520_py2-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42297 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520/client.py
+-rw-r--r--   0 root         (0) root         (0)   238967 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2023-06-28 06:54:03.000000 alibabacloud_linkcard20210520_py2-1.0.9/setup.py
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/ChangeLog.md` & `alibabacloud_linkcard20210520_py2-1.0.9/ChangeLog.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-12 Version: 1.0.8
+- Generated python2 2021-05-20 for Linkcard.
+
 2023-03-14 Version: 1.0.7
 - Generated python2 2021-05-20 for Linkcard.
 
 2023-01-11 Version: 1.0.6
 - Generated python2 2021-05-20 for Linkcard.
 
 2022-12-06 Version: 1.0.5
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/LICENSE` & `alibabacloud_linkcard20210520_py2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/PKG-INFO` & `alibabacloud_linkcard20210520_py2-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkcard20210520_py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Linkcard (20210520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/README-CN.md` & `alibabacloud_linkcard20210520_py2-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/README.md` & `alibabacloud_linkcard20210520_py2-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/client.py` & `alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,14 +86,16 @@
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.msg_notify):
             query['MsgNotify'] = request.msg_notify
         if not UtilClient.is_unset(request.serial_no):
             query['SerialNo'] = request.serial_no
         if not UtilClient.is_unset(request.source):
             query['Source'] = request.source
+        if not UtilClient.is_unset(request.url_insecurity_force):
+            query['UrlInsecurityForce'] = request.url_insecurity_force
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='AddDirectionalAddress',
             version='2021-05-20',
             protocol='HTTPS',
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520/models.py` & `alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,21 +222,23 @@
         if m.get('body') is not None:
             temp_model = AddCardToDirectionalGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class AddDirectionalAddressRequest(TeaModel):
-    def __init__(self, address=None, address_type=None, group_id=None, msg_notify=None, serial_no=None, source=None):
+    def __init__(self, address=None, address_type=None, group_id=None, msg_notify=None, serial_no=None, source=None,
+                 url_insecurity_force=None):
         self.address = address  # type: str
         self.address_type = address_type  # type: str
         self.group_id = group_id  # type: str
         self.msg_notify = msg_notify  # type: bool
         self.serial_no = serial_no  # type: str
         self.source = source  # type: str
+        self.url_insecurity_force = url_insecurity_force  # type: bool
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(AddDirectionalAddressRequest, self).to_map()
         if _map is not None:
@@ -251,14 +253,16 @@
             result['GroupId'] = self.group_id
         if self.msg_notify is not None:
             result['MsgNotify'] = self.msg_notify
         if self.serial_no is not None:
             result['SerialNo'] = self.serial_no
         if self.source is not None:
             result['Source'] = self.source
+        if self.url_insecurity_force is not None:
+            result['UrlInsecurityForce'] = self.url_insecurity_force
         return result
 
     def from_map(self, m=None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
         if m.get('AddressType') is not None:
@@ -267,14 +271,16 @@
             self.group_id = m.get('GroupId')
         if m.get('MsgNotify') is not None:
             self.msg_notify = m.get('MsgNotify')
         if m.get('SerialNo') is not None:
             self.serial_no = m.get('SerialNo')
         if m.get('Source') is not None:
             self.source = m.get('Source')
+        if m.get('UrlInsecurityForce') is not None:
+            self.url_insecurity_force = m.get('UrlInsecurityForce')
         return self
 
 
 class AddDirectionalAddressResponseBody(TeaModel):
     def __init__(self, code=None, data=None, error_message=None, localized_message=None, request_id=None,
                  success=None):
         self.code = code  # type: str
@@ -3126,24 +3132,25 @@
         if m.get('Date') is not None:
             self.date = m.get('Date')
         return self
 
 
 class GetCredentialPoolStatisticsResponseBodyData(TeaModel):
     def __init__(self, card_active_num=None, card_total_num=None, credential_instance_id=None, credential_no=None,
-                 credential_type=None, effective_available_flow=None, effective_total_flow=None, month_feature_fee=None,
-                 month_used_amount=None, pool_avaiable=None, pool_grand_total=None, pool_grand_total_used=None, pool_out_used=None,
-                 pool_used=None, sms_used=None):
+                 credential_type=None, effective_available_flow=None, effective_total_flow=None, month_exceed_fee=None,
+                 month_feature_fee=None, month_used_amount=None, pool_avaiable=None, pool_grand_total=None,
+                 pool_grand_total_used=None, pool_out_used=None, pool_used=None, sms_used=None):
         self.card_active_num = card_active_num  # type: long
         self.card_total_num = card_total_num  # type: long
         self.credential_instance_id = credential_instance_id  # type: str
         self.credential_no = credential_no  # type: str
         self.credential_type = credential_type  # type: str
         self.effective_available_flow = effective_available_flow  # type: str
         self.effective_total_flow = effective_total_flow  # type: str
+        self.month_exceed_fee = month_exceed_fee  # type: long
         self.month_feature_fee = month_feature_fee  # type: long
         self.month_used_amount = month_used_amount  # type: long
         self.pool_avaiable = pool_avaiable  # type: str
         self.pool_grand_total = pool_grand_total  # type: str
         self.pool_grand_total_used = pool_grand_total_used  # type: str
         self.pool_out_used = pool_out_used  # type: str
         self.pool_used = pool_used  # type: str
@@ -3168,14 +3175,16 @@
             result['CredentialNO'] = self.credential_no
         if self.credential_type is not None:
             result['CredentialType'] = self.credential_type
         if self.effective_available_flow is not None:
             result['EffectiveAvailableFlow'] = self.effective_available_flow
         if self.effective_total_flow is not None:
             result['EffectiveTotalFlow'] = self.effective_total_flow
+        if self.month_exceed_fee is not None:
+            result['MonthExceedFee'] = self.month_exceed_fee
         if self.month_feature_fee is not None:
             result['MonthFeatureFee'] = self.month_feature_fee
         if self.month_used_amount is not None:
             result['MonthUsedAmount'] = self.month_used_amount
         if self.pool_avaiable is not None:
             result['PoolAvaiable'] = self.pool_avaiable
         if self.pool_grand_total is not None:
@@ -3202,14 +3211,16 @@
             self.credential_no = m.get('CredentialNO')
         if m.get('CredentialType') is not None:
             self.credential_type = m.get('CredentialType')
         if m.get('EffectiveAvailableFlow') is not None:
             self.effective_available_flow = m.get('EffectiveAvailableFlow')
         if m.get('EffectiveTotalFlow') is not None:
             self.effective_total_flow = m.get('EffectiveTotalFlow')
+        if m.get('MonthExceedFee') is not None:
+            self.month_exceed_fee = m.get('MonthExceedFee')
         if m.get('MonthFeatureFee') is not None:
             self.month_feature_fee = m.get('MonthFeatureFee')
         if m.get('MonthUsedAmount') is not None:
             self.month_used_amount = m.get('MonthUsedAmount')
         if m.get('PoolAvaiable') is not None:
             self.pool_avaiable = m.get('PoolAvaiable')
         if m.get('PoolGrandTotal') is not None:
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO` & `alibabacloud_linkcard20210520_py2-1.0.9/alibabacloud_linkcard20210520_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkcard20210520-py2
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Linkcard (20210520) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkcard20210520_py2-1.0.8/setup.py` & `alibabacloud_linkcard20210520_py2-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkcard20210520_py2.
 
-Created on 12/04/2023
+Created on 28/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkcard20210520"
 NAME = "alibabacloud_linkcard20210520_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Linkcard (20210520) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

