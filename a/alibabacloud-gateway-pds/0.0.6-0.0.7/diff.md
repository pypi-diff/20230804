# Comparing `tmp/alibabacloud_gateway_pds-0.0.6.tar.gz` & `tmp/alibabacloud_gateway_pds-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_pds-0.0.6.tar", last modified: Fri Apr 14 06:45:06 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_pds-0.0.7.tar", last modified: Fri Aug  4 07:12:58 2023, max compression
```

## Comparing `alibabacloud_gateway_pds-0.0.6.tar` & `alibabacloud_gateway_pds-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      886 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18288 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      886 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2865 2023-04-14 06:45:06.000000 alibabacloud_gateway_pds-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds-0.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18390 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      886 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      319 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      383 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2865 2023-08-04 07:12:57.000000 alibabacloud_gateway_pds-0.0.7/setup.py
```

### Comparing `alibabacloud_gateway_pds-0.0.6/PKG-INFO` & `alibabacloud_gateway_pds-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_pds
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alibaba Cloud PDS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds
```

### Comparing `alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds/client.py` & `alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     request.stream = json_obj
                     request.headers['content-type'] = 'application/json; charset=utf-8'
                 else:
                     m = UtilClient.assert_as_map(request.body)
                     form_obj = OpenApiUtilClient.to_form(m)
                     request.stream = form_obj
                     request.headers['content-type'] = 'application/x-www-form-urlencoded'
-        if not UtilClient.equal_string(request.auth_type, 'Anonymous'):
+        if not UtilClient.equal_string(request.auth_type, 'Anonymous') and not UtilClient.is_unset(request.credential):
             credential = request.credential
             auth_type = credential.get_type()
             if UtilClient.equal_string(auth_type, 'bearer'):
                 bearer_token = credential.get_bearer_token()
                 request.headers['x-acs-bearer-token'] = bearer_token
                 request.headers['Authorization'] = f'Bearer {bearer_token}'
             else:
@@ -112,15 +112,15 @@
                     request.stream = json_obj
                     request.headers['content-type'] = 'application/json; charset=utf-8'
                 else:
                     m = UtilClient.assert_as_map(request.body)
                     form_obj = OpenApiUtilClient.to_form(m)
                     request.stream = form_obj
                     request.headers['content-type'] = 'application/x-www-form-urlencoded'
-        if not UtilClient.equal_string(request.auth_type, 'Anonymous'):
+        if not UtilClient.equal_string(request.auth_type, 'Anonymous') and not UtilClient.is_unset(request.credential):
             credential = request.credential
             auth_type = credential.get_type()
             if UtilClient.equal_string(auth_type, 'bearer'):
                 bearer_token = credential.get_bearer_token()
                 request.headers['x-acs-bearer-token'] = bearer_token
                 request.headers['Authorization'] = f'Bearer {bearer_token}'
             else:
@@ -384,15 +384,15 @@
         separator = ''
         for key in sorted_headers_array:
             lower_key = StringClient.to_lower(key)
             if StringClient.has_prefix(lower_key, 'x-acs-'):
                 if not StringClient.contains(tmp, lower_key):
                     tmp = f'{tmp}{separator}{lower_key}'
                     separator = ';'
-        return StringClient.split(tmp, ';', 0)
+        return StringClient.split(tmp, ';', None)
 
     async def get_signed_headers_async(
         self,
         headers: Dict[str, str],
     ) -> List[str]:
         headers_array = MapClient.key_set(headers)
         sorted_headers_array = ArrayClient.asc_sort(headers_array)
@@ -400,8 +400,8 @@
         separator = ''
         for key in sorted_headers_array:
             lower_key = StringClient.to_lower(key)
             if StringClient.has_prefix(lower_key, 'x-acs-'):
                 if not StringClient.contains(tmp, lower_key):
                     tmp = f'{tmp}{separator}{lower_key}'
                     separator = ';'
-        return StringClient.split(tmp, ';', 0)
+        return StringClient.split(tmp, ';', None)
```

### Comparing `alibabacloud_gateway_pds-0.0.6/alibabacloud_gateway_pds.egg-info/PKG-INFO` & `alibabacloud_gateway_pds-0.0.7/alibabacloud_gateway_pds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-pds
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alibaba Cloud PDS SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds
```

### Comparing `alibabacloud_gateway_pds-0.0.6/setup.py` & `alibabacloud_gateway_pds-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,36 +20,36 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_pds.
 
-Created on 14/04/2023
+Created on 04/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_pds"
 NAME = "alibabacloud_gateway_pds" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PDS SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-gateway"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_gateway_spi>=0.0.1, <1.0.0",
-    "alibabacloud_credentials>=0.2.0, <1.0.0",
-    "alibabacloud_tea_util>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.1.6, <1.0.0",
-    "alibabacloud_darabonba_encode_util>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_signature_util>=0.0.3, <1.0.0",
+    "alibabacloud_credentials>=0.3.1, <1.0.0",
+    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
+    "alibabacloud_darabonba_encode_util>=0.0.2, <1.0.0",
+    "alibabacloud_darabonba_signature_util>=0.0.4, <1.0.0",
     "alibabacloud_darabonba_string>=0.0.4, <1.0.0",
     "alibabacloud_darabonba_map>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_array>=0.0.5, <1.0.0"
+    "alibabacloud_darabonba_array>=0.1.0, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

