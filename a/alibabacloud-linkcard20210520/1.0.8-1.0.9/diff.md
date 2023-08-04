# Comparing `tmp/alibabacloud_linkcard20210520-1.0.8.tar.gz` & `tmp/alibabacloud_linkcard20210520-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkcard20210520-1.0.8.tar", last modified: Wed Apr 12 07:08:47 2023, max compression
+gzip compressed data, was "dist/alibabacloud_linkcard20210520-1.0.9.tar", last modified: Wed Jun 28 06:54:47 2023, max compression
```

## Comparing `alibabacloud_linkcard20210520-1.0.8.tar` & `alibabacloud_linkcard20210520-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      540 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520/__init__.py
--rw-r--r--   0 root         (0) root         (0)   101316 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520/client.py
--rw-r--r--   0 root         (0) root         (0)   236436 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2023-04-12 07:08:47.000000 alibabacloud_linkcard20210520-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:54:47.000000 alibabacloud_linkcard20210520-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-28 06:54:47.000000 alibabacloud_linkcard20210520-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:54:47.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101590 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520/client.py
+-rw-r--r--   0 root         (0) root         (0)   237077 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 06:54:47.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-28 06:54:47.000000 alibabacloud_linkcard20210520-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2023-06-28 06:54:46.000000 alibabacloud_linkcard20210520-1.0.9/setup.py
```

### Comparing `alibabacloud_linkcard20210520-1.0.8/ChangeLog.md` & `alibabacloud_linkcard20210520-1.0.9/ChangeLog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-04-12 Version: 1.0.8
+- Generated python 2021-05-20 for Linkcard.
+
 2023-03-14 Version: 1.0.7
 - Generated python 2021-05-20 for Linkcard.
 
 2023-01-11 Version: 1.0.6
 - Generated python 2021-05-20 for Linkcard.
 
 2022-12-06 Version: 1.0.5
```

### Comparing `alibabacloud_linkcard20210520-1.0.8/LICENSE` & `alibabacloud_linkcard20210520-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520-1.0.8/PKG-INFO` & `alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_linkcard20210520
-Version: 1.0.8
+Name: alibabacloud-linkcard20210520
+Version: 1.0.9
 Summary: Alibaba Cloud Linkcard (20210520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkcard20210520-1.0.8/README-CN.md` & `alibabacloud_linkcard20210520-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520-1.0.8/README.md` & `alibabacloud_linkcard20210520-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520/client.py` & `alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,16 @@
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
@@ -197,14 +199,16 @@
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

### Comparing `alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520/models.py` & `alibabacloud_linkcard20210520-1.0.9/alibabacloud_linkcard20210520/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -261,21 +261,23 @@
         self,
         address: str = None,
         address_type: str = None,
         group_id: str = None,
         msg_notify: bool = None,
         serial_no: str = None,
         source: str = None,
+        url_insecurity_force: bool = None,
     ):
         self.address = address
         self.address_type = address_type
         self.group_id = group_id
         self.msg_notify = msg_notify
         self.serial_no = serial_no
         self.source = source
+        self.url_insecurity_force = url_insecurity_force
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -290,14 +292,16 @@
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
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Address') is not None:
             self.address = m.get('Address')
         if m.get('AddressType') is not None:
@@ -306,14 +310,16 @@
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
     def __init__(
         self,
         code: str = None,
@@ -3563,14 +3569,15 @@
         card_active_num: int = None,
         card_total_num: int = None,
         credential_instance_id: str = None,
         credential_no: str = None,
         credential_type: str = None,
         effective_available_flow: str = None,
         effective_total_flow: str = None,
+        month_exceed_fee: int = None,
         month_feature_fee: int = None,
         month_used_amount: int = None,
         pool_avaiable: str = None,
         pool_grand_total: str = None,
         pool_grand_total_used: str = None,
         pool_out_used: str = None,
         pool_used: str = None,
@@ -3579,14 +3586,15 @@
         self.card_active_num = card_active_num
         self.card_total_num = card_total_num
         self.credential_instance_id = credential_instance_id
         self.credential_no = credential_no
         self.credential_type = credential_type
         self.effective_available_flow = effective_available_flow
         self.effective_total_flow = effective_total_flow
+        self.month_exceed_fee = month_exceed_fee
         self.month_feature_fee = month_feature_fee
         self.month_used_amount = month_used_amount
         self.pool_avaiable = pool_avaiable
         self.pool_grand_total = pool_grand_total
         self.pool_grand_total_used = pool_grand_total_used
         self.pool_out_used = pool_out_used
         self.pool_used = pool_used
@@ -3611,14 +3619,16 @@
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
@@ -3645,14 +3655,16 @@
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

### Comparing `alibabacloud_linkcard20210520-1.0.8/alibabacloud_linkcard20210520.egg-info/PKG-INFO` & `alibabacloud_linkcard20210520-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-linkcard20210520
-Version: 1.0.8
+Name: alibabacloud_linkcard20210520
+Version: 1.0.9
 Summary: Alibaba Cloud Linkcard (20210520) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkcard20210520-1.0.8/setup.py` & `alibabacloud_linkcard20210520-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkcard20210520.
 
-Created on 12/04/2023
+Created on 28/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkcard20210520"
 NAME = "alibabacloud_linkcard20210520" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Linkcard (20210520) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.9, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

