# Comparing `tmp/alibabacloud_airticketopen20230117-3.0.0.tar.gz` & `tmp/alibabacloud_airticketopen20230117-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_airticketopen20230117-3.0.0.tar", last modified: Wed Jul  5 03:52:32 2023, max compression
+gzip compressed data, was "dist/alibabacloud_airticketopen20230117-3.0.1.tar", last modified: Fri Aug  4 06:03:09 2023, max compression
```

## Comparing `alibabacloud_airticketopen20230117-3.0.0.tar` & `alibabacloud_airticketopen20230117-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104846 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/client.py
--rw-r--r--   0 root         (0) root         (0)   507628 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-05 03:52:32.000000 alibabacloud_airticketopen20230117-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2660 2023-07-05 03:52:31.000000 alibabacloud_airticketopen20230117-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:03:09.000000 alibabacloud_airticketopen20230117-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)      380 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-08-04 06:03:09.000000 alibabacloud_airticketopen20230117-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:03:09.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108950 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117/client.py
+-rw-r--r--   0 root         (0) root         (0)   513856 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:03:09.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-04 06:03:09.000000 alibabacloud_airticketopen20230117-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2661 2023-08-04 06:03:08.000000 alibabacloud_airticketopen20230117-3.0.1/setup.py
```

### Comparing `alibabacloud_airticketopen20230117-3.0.0/LICENSE` & `alibabacloud_airticketopen20230117-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-3.0.0/PKG-INFO` & `alibabacloud_airticketopen20230117-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_airticketopen20230117
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-3.0.0/README-CN.md` & `alibabacloud_airticketopen20230117-3.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-3.0.0/README.md` & `alibabacloud_airticketopen20230117-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/client.py` & `alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2226,7 +2226,97 @@
     async def ticketing_async(
         self,
         request: airticket_open_20230117_models.TicketingRequest,
     ) -> airticket_open_20230117_models.TicketingResponse:
         runtime = util_models.RuntimeOptions()
         headers = airticket_open_20230117_models.TicketingHeaders()
         return await self.ticketing_with_options_async(request, headers, runtime)
+
+    def ticketing_check_with_options(
+        self,
+        request: airticket_open_20230117_models.TicketingCheckRequest,
+        headers: airticket_open_20230117_models.TicketingCheckHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> airticket_open_20230117_models.TicketingCheckResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.order_num):
+            body['order_num'] = request.order_num
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_airticket_access_token):
+            real_headers['x-acs-airticket-access-token'] = UtilClient.to_jsonstring(headers.x_acs_airticket_access_token)
+        if not UtilClient.is_unset(headers.x_acs_airticket_language):
+            real_headers['x-acs-airticket-language'] = UtilClient.to_jsonstring(headers.x_acs_airticket_language)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TicketingCheck',
+            version='2023-01-17',
+            protocol='HTTPS',
+            pathname=f'/airticket/v1/trade/action-ticketing-check',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            airticket_open_20230117_models.TicketingCheckResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def ticketing_check_with_options_async(
+        self,
+        request: airticket_open_20230117_models.TicketingCheckRequest,
+        headers: airticket_open_20230117_models.TicketingCheckHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> airticket_open_20230117_models.TicketingCheckResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.order_num):
+            body['order_num'] = request.order_num
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_airticket_access_token):
+            real_headers['x-acs-airticket-access-token'] = UtilClient.to_jsonstring(headers.x_acs_airticket_access_token)
+        if not UtilClient.is_unset(headers.x_acs_airticket_language):
+            real_headers['x-acs-airticket-language'] = UtilClient.to_jsonstring(headers.x_acs_airticket_language)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='TicketingCheck',
+            version='2023-01-17',
+            protocol='HTTPS',
+            pathname=f'/airticket/v1/trade/action-ticketing-check',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            airticket_open_20230117_models.TicketingCheckResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def ticketing_check(
+        self,
+        request: airticket_open_20230117_models.TicketingCheckRequest,
+    ) -> airticket_open_20230117_models.TicketingCheckResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = airticket_open_20230117_models.TicketingCheckHeaders()
+        return self.ticketing_check_with_options(request, headers, runtime)
+
+    async def ticketing_check_async(
+        self,
+        request: airticket_open_20230117_models.TicketingCheckRequest,
+    ) -> airticket_open_20230117_models.TicketingCheckResponse:
+        runtime = util_models.RuntimeOptions()
+        headers = airticket_open_20230117_models.TicketingCheckHeaders()
+        return await self.ticketing_check_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117/models.py` & `alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13629,7 +13629,210 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TicketingResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TicketingCheckHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_airticket_access_token: str = None,
+        x_acs_airticket_language: str = None,
+    ):
+        self.common_headers = common_headers
+        # access_token
+        self.x_acs_airticket_access_token = x_acs_airticket_access_token
+        self.x_acs_airticket_language = x_acs_airticket_language
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_airticket_access_token is not None:
+            result['x-acs-airticket-access-token'] = self.x_acs_airticket_access_token
+        if self.x_acs_airticket_language is not None:
+            result['x-acs-airticket-language'] = self.x_acs_airticket_language
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-airticket-access-token') is not None:
+            self.x_acs_airticket_access_token = m.get('x-acs-airticket-access-token')
+        if m.get('x-acs-airticket-language') is not None:
+            self.x_acs_airticket_language = m.get('x-acs-airticket-language')
+        return self
+
+
+class TicketingCheckRequest(TeaModel):
+    def __init__(
+        self,
+        order_num: int = None,
+    ):
+        self.order_num = order_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_num is not None:
+            result['order_num'] = self.order_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('order_num') is not None:
+            self.order_num = m.get('order_num')
+        return self
+
+
+class TicketingCheckResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        order_num: int = None,
+    ):
+        self.order_num = order_num
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.order_num is not None:
+            result['order_num'] = self.order_num
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('order_num') is not None:
+            self.order_num = m.get('order_num')
+        return self
+
+
+class TicketingCheckResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        data: TicketingCheckResponseBodyData = None,
+        error_code: str = None,
+        error_data: Any = None,
+        error_msg: str = None,
+        status: int = None,
+        success: bool = None,
+    ):
+        self.request_id = request_id
+        self.data = data
+        self.error_code = error_code
+        self.error_data = error_data
+        self.error_msg = error_msg
+        self.status = status
+        self.success = success
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        if self.error_code is not None:
+            result['error_code'] = self.error_code
+        if self.error_data is not None:
+            result['error_data'] = self.error_data
+        if self.error_msg is not None:
+            result['error_msg'] = self.error_msg
+        if self.status is not None:
+            result['status'] = self.status
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('data') is not None:
+            temp_model = TicketingCheckResponseBodyData()
+            self.data = temp_model.from_map(m['data'])
+        if m.get('error_code') is not None:
+            self.error_code = m.get('error_code')
+        if m.get('error_data') is not None:
+            self.error_data = m.get('error_data')
+        if m.get('error_msg') is not None:
+            self.error_msg = m.get('error_msg')
+        if m.get('status') is not None:
+            self.status = m.get('status')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class TicketingCheckResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TicketingCheckResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TicketingCheckResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_airticketopen20230117-3.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO` & `alibabacloud_airticketopen20230117-3.0.1/alibabacloud_airticketopen20230117.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-airticketopen20230117
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-3.0.0/setup.py` & `alibabacloud_airticketopen20230117-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_airticketopen20230117.
 
-Created on 05/07/2023
+Created on 04/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_airticketopen20230117"
 NAME = "alibabacloud_airticketopen20230117" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud airticketOpen (20230117) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

