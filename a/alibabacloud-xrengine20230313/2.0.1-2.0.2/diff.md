# Comparing `tmp/alibabacloud_xrengine20230313-2.0.1.tar.gz` & `tmp/alibabacloud_xrengine20230313-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.0.1.tar", last modified: Thu Aug  3 09:19:00 2023, max compression
+gzip compressed data, was "dist/alibabacloud_xrengine20230313-2.0.2.tar", last modified: Fri Aug  4 05:35:53 2023, max compression
```

## Comparing `alibabacloud_xrengine20230313-2.0.1.tar` & `alibabacloud_xrengine20230313-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/
--rw-r--r--   0 root         (0) root         (0)      217 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81239 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/client.py
--rw-r--r--   0 root         (0) root         (0)   271529 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-03 09:19:00.000000 alibabacloud_xrengine20230313-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-08-03 09:18:59.000000 alibabacloud_xrengine20230313-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:35:53.000000 alibabacloud_xrengine20230313-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)      266 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-04 05:35:53.000000 alibabacloud_xrengine20230313-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:35:53.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84565 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313/client.py
+-rw-r--r--   0 root         (0) root         (0)   278335 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 05:35:53.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-04 05:35:53.000000 alibabacloud_xrengine20230313-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-08-04 05:35:52.000000 alibabacloud_xrengine20230313-2.0.2/setup.py
```

### Comparing `alibabacloud_xrengine20230313-2.0.1/LICENSE` & `alibabacloud_xrengine20230313-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.0.1/PKG-INFO` & `alibabacloud_xrengine20230313-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_xrengine20230313
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-2.0.1/README-CN.md` & `alibabacloud_xrengine20230313-2.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.0.1/README.md` & `alibabacloud_xrengine20230313-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/client.py` & `alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1679,14 +1679,96 @@
     async def pop_list_object_project_async(
         self,
         request: xr_engine_20230313_models.PopListObjectProjectRequest,
     ) -> xr_engine_20230313_models.PopListObjectProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.pop_list_object_project_with_options_async(request, runtime)
 
+    def pop_list_pak_render_expression_with_options(
+        self,
+        request: xr_engine_20230313_models.PopListPakRenderExpressionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopListPakRenderExpressionResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.list_status):
+            query['ListStatus'] = request.list_status
+        body = {}
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopListPakRenderExpression',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopListPakRenderExpressionResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def pop_list_pak_render_expression_with_options_async(
+        self,
+        request: xr_engine_20230313_models.PopListPakRenderExpressionRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> xr_engine_20230313_models.PopListPakRenderExpressionResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.list_status):
+            query['ListStatus'] = request.list_status
+        body = {}
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.size):
+            body['Size'] = request.size
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='PopListPakRenderExpression',
+            version='2023-03-13',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            xr_engine_20230313_models.PopListPakRenderExpressionResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def pop_list_pak_render_expression(
+        self,
+        request: xr_engine_20230313_models.PopListPakRenderExpressionRequest,
+    ) -> xr_engine_20230313_models.PopListPakRenderExpressionResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.pop_list_pak_render_expression_with_options(request, runtime)
+
+    async def pop_list_pak_render_expression_async(
+        self,
+        request: xr_engine_20230313_models.PopListPakRenderExpressionRequest,
+    ) -> xr_engine_20230313_models.PopListPakRenderExpressionResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.pop_list_pak_render_expression_with_options_async(request, runtime)
+
     def pop_list_text_to_avatar_project_with_options(
         self,
         request: xr_engine_20230313_models.PopListTextToAvatarProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> xr_engine_20230313_models.PopListTextToAvatarProjectResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313/models.py` & `alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6255,14 +6255,237 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = PopListObjectProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class PopListPakRenderExpressionRequest(TeaModel):
+    def __init__(
+        self,
+        current: int = None,
+        list_status: str = None,
+        size: int = None,
+    ):
+        self.current = current
+        self.list_status = list_status
+        self.size = size
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
+        if self.current is not None:
+            result['Current'] = self.current
+        if self.list_status is not None:
+            result['ListStatus'] = self.list_status
+        if self.size is not None:
+            result['Size'] = self.size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        if m.get('ListStatus') is not None:
+            self.list_status = m.get('ListStatus')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
+        return self
+
+
+class PopListPakRenderExpressionResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        cover_url: str = None,
+        ext: str = None,
+        file_url: str = None,
+        id: str = None,
+        intro: str = None,
+        name: str = None,
+    ):
+        self.cover_url = cover_url
+        self.ext = ext
+        self.file_url = file_url
+        self.id = id
+        self.intro = intro
+        self.name = name
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
+        if self.cover_url is not None:
+            result['CoverUrl'] = self.cover_url
+        if self.ext is not None:
+            result['Ext'] = self.ext
+        if self.file_url is not None:
+            result['FileUrl'] = self.file_url
+        if self.id is not None:
+            result['Id'] = self.id
+        if self.intro is not None:
+            result['Intro'] = self.intro
+        if self.name is not None:
+            result['Name'] = self.name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CoverUrl') is not None:
+            self.cover_url = m.get('CoverUrl')
+        if m.get('Ext') is not None:
+            self.ext = m.get('Ext')
+        if m.get('FileUrl') is not None:
+            self.file_url = m.get('FileUrl')
+        if m.get('Id') is not None:
+            self.id = m.get('Id')
+        if m.get('Intro') is not None:
+            self.intro = m.get('Intro')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        return self
+
+
+class PopListPakRenderExpressionResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        current: int = None,
+        data: List[PopListPakRenderExpressionResponseBodyData] = None,
+        message: str = None,
+        pages: int = None,
+        request_id: str = None,
+        size: int = None,
+        success: bool = None,
+        total: int = None,
+    ):
+        self.code = code
+        self.current = current
+        self.data = data
+        self.message = message
+        self.pages = pages
+        self.request_id = request_id
+        self.size = size
+        self.success = success
+        self.total = total
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.current is not None:
+            result['Current'] = self.current
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.pages is not None:
+            result['Pages'] = self.pages
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.size is not None:
+            result['Size'] = self.size
+        if self.success is not None:
+            result['Success'] = self.success
+        if self.total is not None:
+            result['Total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = PopListPakRenderExpressionResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Pages') is not None:
+            self.pages = m.get('Pages')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Size') is not None:
+            self.size = m.get('Size')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        if m.get('Total') is not None:
+            self.total = m.get('Total')
+        return self
+
+
+class PopListPakRenderExpressionResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: PopListPakRenderExpressionResponseBody = None,
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
+            temp_model = PopListPakRenderExpressionResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class PopListTextToAvatarProjectRequest(TeaModel):
     def __init__(
         self,
         current: int = None,
         jwt_token: str = None,
         size: int = None,
         sort_field: str = None,
```

### Comparing `alibabacloud_xrengine20230313-2.0.1/alibabacloud_xrengine20230313.egg-info/PKG-INFO` & `alibabacloud_xrengine20230313-2.0.2/alibabacloud_xrengine20230313.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-xrengine20230313
-Version: 2.0.1
+Version: 2.0.2
 Summary: Alibaba Cloud xrEngine (20230313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_xrengine20230313-2.0.1/setup.py` & `alibabacloud_xrengine20230313-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_xrengine20230313.
 
-Created on 03/08/2023
+Created on 04/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_xrengine20230313"
 NAME = "alibabacloud_xrengine20230313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud xrEngine (20230313) SDK Library for Python"
```

