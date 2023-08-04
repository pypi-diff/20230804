# Comparing `tmp/alibabacloud_gateway_pds_py2-0.0.6.tar.gz` & `tmp/alibabacloud_gateway_pds_py2-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gateway_pds_py2-0.0.6.tar", last modified: Fri Apr 14 06:45:09 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gateway_pds_py2-0.0.7.tar", last modified: Fri Aug  4 07:12:59 2023, max compression
```

## Comparing `alibabacloud_gateway_pds_py2-0.0.6.tar` & `alibabacloud_gateway_pds_py2-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9440 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      419 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3177 2023-04-14 06:45:09.000000 alibabacloud_gateway_pds_py2-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9491 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      339 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      419 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 07:12:59.000000 alibabacloud_gateway_pds_py2-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-08-04 07:12:58.000000 alibabacloud_gateway_pds_py2-0.0.7/setup.py
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.6/PKG-INFO` & `alibabacloud_gateway_pds_py2-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gateway_pds_py2
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alibaba Cloud PDS SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds,py2
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds/client.py` & `alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
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
                 request.headers['Authorization'] = 'Bearer %s' % TeaConverter.to_unicode(bearer_token)
             else:
@@ -167,8 +167,8 @@
         separator = ''
         for key in sorted_headers_array:
             lower_key = StringClient.to_lower(key)
             if StringClient.has_prefix(lower_key, 'x-acs-'):
                 if not StringClient.contains(tmp, lower_key):
                     tmp = '%s%s%s' % (TeaConverter.to_unicode(tmp), TeaConverter.to_unicode(separator), TeaConverter.to_unicode(lower_key))
                     separator = ';'
-        return StringClient.split(tmp, ';', 0)
+        return StringClient.split(tmp, ';', None)
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.6/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO` & `alibabacloud_gateway_pds_py2-0.0.7/alibabacloud_gateway_pds_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gateway-pds-py2
-Version: 0.0.6
+Version: 0.0.7
 Summary: Alibaba Cloud PDS SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-gateway
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,gateway,pds,py2
```

### Comparing `alibabacloud_gateway_pds_py2-0.0.6/setup.py` & `alibabacloud_gateway_pds_py2-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,36 +21,36 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gateway_pds_py2.
 
-Created on 14/04/2023
+Created on 04/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gateway_pds"
 NAME = "alibabacloud_gateway_pds_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud PDS SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-gateway"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_gateway_spi_py2>=0.0.1, <1.0.0",
-    "alibabacloud_credentials_py2>=0.0.1, <1.0.0",
-    "alibabacloud_tea_util_py2>=0.0.6, <1.0.0",
-    "alibabacloud_openapi_util_py2>=0.0.8, <1.0.0",
-    "alibabacloud_darabonba_encode_util_py2>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_signature_util_py2>=0.0.3, <1.0.0",
+    "alibabacloud_credentials_py2>=0.1.1, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.7, <1.0.0",
+    "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
+    "alibabacloud_darabonba_encode_util_py2>=0.0.2, <1.0.0",
+    "alibabacloud_darabonba_signature_util_py2>=0.0.4, <1.0.0",
     "alibabacloud_darabonba_string_py2>=0.0.4, <1.0.0",
-    "alibabacloud_darabonba_map_py2>=0.0.1, <1.0.0",
-    "alibabacloud_darabonba_array_py2>=0.0.5, <1.0.0"
+    "alibabacloud_darabonba_map_py2>=0.0.2, <1.0.0",
+    "alibabacloud_darabonba_array_py2>=0.1.0, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 
 if os.path.exists('./README.md'):
     if sys.version_info.major == 2:
         with open("README.md") as fp:
```

