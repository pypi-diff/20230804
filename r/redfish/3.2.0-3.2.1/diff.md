# Comparing `tmp/redfish-3.2.0.tar.gz` & `tmp/redfish-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish-3.2.0.tar", last modified: Thu Jul 27 14:57:56 2023, max compression
+gzip compressed data, was "redfish-3.2.1.tar", last modified: Fri Aug  4 19:42:37 2023, max compression
```

## Comparing `redfish-3.2.0.tar` & `redfish-3.2.1.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.884111 redfish-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 14:57:38.000000 redfish-3.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-27 14:57:38.000000 redfish-3.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-27 14:57:56.884111 redfish-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-07-27 14:57:38.000000 redfish-3.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 14:57:56.884111 redfish-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-27 14:57:49.000000 redfish-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-27 14:57:49.000000 redfish-3.2.0/src/redfish/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/discovery/discovery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42047 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/rest/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.884111 redfish-3.2.0/src/redfish/ris/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/ris.py
--rw-r--r--   0 runner    (1001) docker     (123)    67528 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/rmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/rmc_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-27 14:57:38.000000 redfish-3.2.0/src/redfish/ris/sharedtypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 14:57:56.880110 redfish-3.2.0/src/redfish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-27 14:57:56.000000 redfish-3.2.0/src/redfish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.610978 redfish-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-04 19:42:26.000000 redfish-3.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-08-04 19:42:26.000000 redfish-3.2.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-08-04 19:42:37.610978 redfish-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-08-04 19:42:26.000000 redfish-3.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:42:37.610978 redfish-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-04 19:42:34.000000 redfish-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/redfish/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-08-04 19:42:34.000000 redfish-3.2.1/src/redfish/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/redfish/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/discovery/discovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/redfish/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/messages/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/redfish/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45240 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/rest/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/redfish/ris/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/ris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/ris/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21137 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/ris/ris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67528 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/ris/rmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23633 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/ris/rmc_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-08-04 19:42:26.000000 redfish-3.2.1/src/redfish/ris/sharedtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:42:37.606978 redfish-3.2.1/src/redfish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-08-04 19:42:37.000000 redfish-3.2.1/src/redfish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-08-04 19:42:37.000000 redfish-3.2.1/src/redfish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:42:37.000000 redfish-3.2.1/src/redfish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-04 19:42:37.000000 redfish-3.2.1/src/redfish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 19:42:37.000000 redfish-3.2.1/src/redfish.egg-info/top_level.txt
```

### Comparing `redfish-3.2.0/AUTHORS.md` & `redfish-3.2.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/LICENSE.md` & `redfish-3.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/PKG-INFO` & `redfish-3.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: redfish
-Version: 3.2.0
-Summary: Redfish Python Library
-Home-page: https://github.com/DMTF/python-redfish-library
-Author: DMTF, https://www.dmtf.org/standards/feedback
-License: BSD 3-clause "New" or "Revised License"
-Keywords: Redfish
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Communications
-Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-License-File: AUTHORS.md
-
 python-redfish-library
 ======================
 
 .. image:: https://img.shields.io/pypi/v/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 .. image:: https://img.shields.io/github/release/DMTF/python-redfish-library.svg?maxAge=2592000
     :target: https://github.com/DMTF/python-redfish-library/releases
@@ -164,14 +148,26 @@
   - A string is used to supply an unstructed body, which may be used in some OEM cases.
 
 * ``headers``: Dictionary.  Additional HTTP headers to supply with the request.
 
   - The key-value pairs in the dictionary are the HTTP header name and the HTTP header value to supply.
   - Example: ``{"If-Match": etag_value}``
 
+* ``timeout``: Number.  The number of seconds to wait for a response before closing the connection for this request.
+
+  - Overrides the timeout value specified when the Redfish object is created for this request.
+  - This can be useful when a particular URI is known to take a long time to respond, such as with firmware updates.
+  - The default value is ``None``, which indicates the object-defined timeout is used.
+
+* ``max_retry``: Number.  The number of retries to perform an operation before giving up for this request.
+
+  - Overrides the max retry value specified when the Redfish object is created for this request.
+  - This can be useful when a particular URI is known to take multiple retries.
+  - The default value is ``None``, which indicates the object-defined max retry count is used.
+
 Working with tasks
 ~~~~~~~~~~~~~~~~~~
 
 POST, PATCH, PUT, and DELETE operations may result in a task, describing an operation with a duration greater than the span of a single request.
 The action message object that ``is_processing`` will return a task that can be accessed reviewed when polled with monitor.
 An example of a POST operation with a possible task is shown below.
```

### Comparing `redfish-3.2.0/README.rst` & `redfish-3.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: redfish
+Version: 3.2.1
+Summary: Redfish Python Library
+Home-page: https://github.com/DMTF/python-redfish-library
+Author: DMTF, https://www.dmtf.org/standards/feedback
+License: BSD 3-clause "New" or "Revised License"
+Keywords: Redfish
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Communications
+Description-Content-Type: text/x-rst
+License-File: LICENSE.md
+License-File: AUTHORS.md
+
 python-redfish-library
 ======================
 
 .. image:: https://img.shields.io/pypi/v/redfish.svg?maxAge=2592000
     :target: https://pypi.python.org/pypi/redfish
 .. image:: https://img.shields.io/github/release/DMTF/python-redfish-library.svg?maxAge=2592000
     :target: https://github.com/DMTF/python-redfish-library/releases
@@ -148,14 +164,26 @@
   - A string is used to supply an unstructed body, which may be used in some OEM cases.
 
 * ``headers``: Dictionary.  Additional HTTP headers to supply with the request.
 
   - The key-value pairs in the dictionary are the HTTP header name and the HTTP header value to supply.
   - Example: ``{"If-Match": etag_value}``
 
+* ``timeout``: Number.  The number of seconds to wait for a response before closing the connection for this request.
+
+  - Overrides the timeout value specified when the Redfish object is created for this request.
+  - This can be useful when a particular URI is known to take a long time to respond, such as with firmware updates.
+  - The default value is ``None``, which indicates the object-defined timeout is used.
+
+* ``max_retry``: Number.  The number of retries to perform an operation before giving up for this request.
+
+  - Overrides the max retry value specified when the Redfish object is created for this request.
+  - This can be useful when a particular URI is known to take multiple retries.
+  - The default value is ``None``, which indicates the object-defined max retry count is used.
+
 Working with tasks
 ~~~~~~~~~~~~~~~~~~
 
 POST, PATCH, PUT, and DELETE operations may result in a task, describing an operation with a duration greater than the span of a single request.
 The action message object that ``is_processing`` will return a task that can be accessed reviewed when polled with monitor.
 An example of a POST operation with a possible task is shown below.
```

### Comparing `redfish-3.2.0/setup.py` & `redfish-3.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='redfish',
-      version='3.2.0',
+      version='3.2.1',
       description='Redfish Python Library',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       author = 'DMTF, https://www.dmtf.org/standards/feedback',
       license='BSD 3-clause "New" or "Revised License"',
       classifiers=[
           'Development Status :: 5 - Production/Stable',
```

### Comparing `redfish-3.2.0/src/redfish/__init__.py` & `redfish-3.2.1/src/redfish/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright Notice:
 # Copyright 2016-2021 DMTF. All rights reserved.
 # License: BSD 3-Clause License. For full text see link:
 # https://github.com/DMTF/python-redfish-library/blob/main/LICENSE.md
 
 """ Redfish restful library """
 
-__all__ = ['rest', 'ris', 'discovery']
-__version__ = "3.2.0"
+__all__ = ['rest', 'ris', 'discovery', 'messages']
+__version__ = "3.2.1"
 
 from redfish.rest.v1 import redfish_client
 from redfish.rest.v1 import AuthMethod
 from redfish.discovery.discovery import discover_ssdp
+from redfish.messages import *
 import logging
 
 def redfish_logger(file_name, log_format, log_level=logging.ERROR):
     formatter = logging.Formatter(log_format)
     fh = logging.FileHandler(file_name)
     fh.setFormatter(formatter)
     logger = logging.getLogger(__name__)
```

### Comparing `redfish-3.2.0/src/redfish/discovery/discovery.py` & `redfish-3.2.1/src/redfish/discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish/rest/v1.py` & `redfish-3.2.1/src/redfish/rest/v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import json
 import base64
 import logging
 import warnings
 import re
 import requests
 import requests_unixsocket
+from redfish.messages import *
 
 from collections import (OrderedDict)
 
 from urllib.parse import urlparse, urlencode, quote
 from io import StringIO
 
 from requests_toolbelt import MultipartEncoder
@@ -603,114 +604,138 @@
                 self.default_prefix, content)
             LOGGER.error(str)
             raise JsonDecodingError(str) from None
 
         self.root = RisObject.parse(root_data)
         self.root_resp = resp
 
-    def get(self, path, args=None, headers=None):
+    def get(self, path, args=None, headers=None, timeout=None, max_retry=None):
         """Perform a GET request
 
         :param path: The URI to access
         :type path: str
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a rest request with method 'Get'
 
         """
         try:
             return self._rest_request(path, method='GET', args=args,
-                                                                headers=headers)
+                                                                headers=headers, timeout=timeout, max_retry=max_retry)
         except ValueError:
             str = "Service responded with invalid JSON at URI {}".format(path)
             LOGGER.error(str)
             raise JsonDecodingError(str) from None
 
-    def head(self, path, args=None, headers=None):
+    def head(self, path, args=None, headers=None, timeout=None, max_retry=None):
         """Perform a HEAD request
 
         :param path: The URI to access
         :type path: str
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a rest request with method 'Head'
 
         """
         return self._rest_request(path, method='HEAD', args=args,
-                                                                headers=headers)
+                                                                headers=headers, timeout=timeout, max_retry=max_retry)
 
-    def post(self, path, args=None, body=None, headers=None):
+    def post(self, path, args=None, body=None, headers=None, timeout=None, max_retry=None):
         """Perform a POST request
 
         :param path: The URI to access
         :type path: str
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
         :type body: dict or list or bytes or str, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a rest request with method 'Post'
 
         """
         return self._rest_request(path, method='POST', args=args, body=body,
-                                                                headers=headers)
+                                                                headers=headers, timeout=timeout, max_retry=max_retry)
 
-    def put(self, path, args=None, body=None, headers=None):
+    def put(self, path, args=None, body=None, headers=None, timeout=None, max_retry=None):
         """Perform a PUT request
 
         :param path: The URI to access
         :type path: str
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
         :type body: dict or list or bytes or str, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a rest request with method 'Put'
 
         """
         return self._rest_request(path, method='PUT', args=args, body=body,
-                                                                headers=headers)
+                                                                headers=headers, timeout=timeout, max_retry=max_retry)
 
-    def patch(self, path, args=None, body=None, headers=None):
+    def patch(self, path, args=None, body=None, headers=None, timeout=None, max_retry=None):
         """Perform a PATCH request
 
         :param path: The URI to access
         :type path: str
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
         :type body: dict or list or bytes or str, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a rest request with method 'Patch'
 
         """
         return self._rest_request(path, method='PATCH', args=args, body=body,
-                                                                headers=headers)
+                                                                headers=headers, timeout=timeout, max_retry=max_retry)
 
-    def delete(self, path, args=None, headers=None):
+    def delete(self, path, args=None, headers=None, timeout=None, max_retry=None):
         """Perform a DELETE request
 
         :param path: The URI to access
         :type path: str
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a rest request with method 'Delete'
 
         """
         return self._rest_request(path, method='DELETE', args=args,
-                                                                headers=headers)
+                                                                headers=headers, timeout=timeout, max_retry=max_retry)
 
     def _get_req_headers(self, headers=None):
         """Get the request headers
 
         :param headers: additional headers to be utilized
         :type headers: dict
         :returns: returns headers
@@ -726,32 +751,42 @@
         headers_keys = set(k.lower() for k in headers)
         if 'accept' not in headers_keys:
             headers['Accept'] = '*/*'
 
         return headers
 
     def _rest_request(self, path, method='GET', args=None, body=None,
-                      headers=None, allow_redirects=True):
+                      headers=None, allow_redirects=True, timeout=None, max_retry=None):
         """Rest request main function
 
         :param path: The URI to access
         :type path: str
         :param method: The HTTP method to invoke on the URI; GET if not provided
         :type method: str, optional
         :param args: The query parameters to provide with the request
         :type args: dict, optional
         :param body: The request body to provide; use a dict for a JSON body, list for multipart forms, bytes for an octet stream, or str for an unstructured request
         :type body: dict or list or bytes or str, optional
         :param headers: Additional HTTP headers to provide in the request
         :type headers: dict, optional
         :param allow_redirects: Controls whether redirects are followed
         :type allow_redirects: bool, optional
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int, optional
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int, optional
         :returns: returns a RestResponse object
 
         """
+        if timeout is None:
+            timeout = self._timeout
+
+        if max_retry is None:
+            max_retry = self._max_retry
+
         headers = self._get_req_headers(headers)
         reqpath = path.replace('//', '/')
 
         if body is not None:
             if isinstance(body, dict) or isinstance(body, list):
                 if headers.get('Content-Type', None) == 'multipart/form-data':
                     # Body contains part values, either as
@@ -782,15 +817,15 @@
                 headers['Content-Type'] = 'application/octet-stream'
                 body = body
             else:
                 headers['Content-Type'] = 'application/x-www-form-urlencoded'
                 body = urlencode(body)
 
             if method == 'PUT':
-                resp = self._rest_request(path=path)
+                resp = self._rest_request(path=path, timeout=timeout, max_retry=max_retry)
 
                 try:
                     if resp.getheader('content-encoding') == 'gzip':
                         buf = StringIO()
                         gfile = gzip.GzipFile(mode='wb', fileobj=buf)
 
                         try:
@@ -832,15 +867,15 @@
                     LOGGER.warning('Use the "body" parameter to supply the request payload.')
 
         restreq = RestRequest(reqpath, method=method, body=body)
 
         attempts = 0
         restresp = None
         cause_exception = None
-        while attempts <= self._max_retry:
+        while attempts <= max_retry:
             if LOGGER.isEnabledFor(logging.DEBUG):
                 headerstr = ''
                 if headers is not None:
                     for header in headers:
                         if header.lower() == "authorization":
                             headerstr += '\t{}: <REDACTED>\n'.format(header)
                         else:
@@ -869,15 +904,15 @@
                     inittime = time.perf_counter()
 
                 # TODO: Migration to requests lost the "CA directory" capability; need to revisit
                 verify = False
                 if self.cafile:
                     verify = self.cafile
                 resp = self._session.request(method.upper(), "{}{}".format(self.__base_url, reqpath), data=body,
-                                             headers=headers, timeout=self._timeout, allow_redirects=allow_redirects,
+                                             headers=headers, timeout=timeout, allow_redirects=allow_redirects,
                                              verify=verify, proxies=self._proxies, params=query_str)
 
                 if sys.version_info < (3, 3):
                     endtime = time.clock()
                 else:
                     endtime = time.perf_counter()
                 LOGGER.info('Response Time for %s to %s: %s seconds.' %
@@ -957,14 +992,18 @@
                                       headers=headers, allow_redirects=False)
 
             LOGGER.info('Login returned code %s: %s', resp.status, resp.text)
 
             self.__session_key = resp.session_key
             self.__session_location = resp.session_location
 
+            message_item = search_message(resp, "Base", "PasswordChangeRequired")
+            if not message_item is None:
+                raise RedfishPasswordChangeRequiredError("Password Change Required\n", message_item["MessageArgs"][0])
+            
             if not self.__session_key and resp.status not in [200, 201, 202, 204]:
                 if resp.status == 401:
                     # Invalid credentials supplied
                     raise InvalidCredentialsError('HTTP 401 Unauthorized returned: Invalid credentials supplied')
                 else:
                     # Other type of error during session creation
                     error_str = resp.text
@@ -1042,36 +1081,40 @@
         except KeyError:
             # While the "Links/Sessions" property is required, we can fallback
             # on the URI hardened in 1.6.0 of the specification if not found
             LOGGER.debug('"Links/Sessions" not found in Service Root.')
             self.login_url = '/redfish/v1/SessionService/Sessions'
 
     def _rest_request(self, path='', method="GET", args=None, body=None,
-                      headers=None, allow_redirects=True):
+                      headers=None, allow_redirects=True, timeout=None, max_retry=None):
         """Rest request for HTTP client
 
         :param path: path within tree
         :type path: str
         :param method: method to be implemented
         :type method: str
         :param args: the arguments for method
         :type args: dict
         :param body: body payload for the rest call
         :type body: dict
         :param headers: provide additional headers
         :type headers: dict
         :param allow_redirects: controls whether redirects are followed
         :type allow_redirects: bool
+        :param timeout: Timeout in seconds for the initial connection for this specific request
+        :type timeout: int
+        :param max_retry: Number of times a request will retry after a timeout for this specific request
+        :type max_retry: int
         :returns: returns a rest request
 
         """
         return super(HttpClient, self)._rest_request(path=path, method=method,
                                                      args=args, body=body,
                                                      headers=headers,
-                                                     allow_redirects=allow_redirects)
+                                                     allow_redirects=allow_redirects, timeout=timeout, max_retry=max_retry)
 
     def _get_req_headers(self, headers=None, providerheader=None):
         """Get the request headers for HTTP client
 
         :param headers: additional headers to be utilized
         :type headers: dict
         :returns: returns request headers
```

### Comparing `redfish-3.2.0/src/redfish/ris/__init__.py` & `redfish-3.2.1/src/redfish/ris/__init__.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish/ris/config.py` & `redfish-3.2.1/src/redfish/ris/config.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish/ris/ris.py` & `redfish-3.2.1/src/redfish/ris/ris.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish/ris/rmc.py` & `redfish-3.2.1/src/redfish/ris/rmc.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish/ris/rmc_helper.py` & `redfish-3.2.1/src/redfish/ris/rmc_helper.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish/ris/sharedtypes.py` & `redfish-3.2.1/src/redfish/ris/sharedtypes.py`

 * *Files identical despite different names*

### Comparing `redfish-3.2.0/src/redfish.egg-info/PKG-INFO` & `redfish-3.2.1/src/redfish.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish
-Version: 3.2.0
+Version: 3.2.1
 Summary: Redfish Python Library
 Home-page: https://github.com/DMTF/python-redfish-library
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
@@ -164,14 +164,26 @@
   - A string is used to supply an unstructed body, which may be used in some OEM cases.
 
 * ``headers``: Dictionary.  Additional HTTP headers to supply with the request.
 
   - The key-value pairs in the dictionary are the HTTP header name and the HTTP header value to supply.
   - Example: ``{"If-Match": etag_value}``
 
+* ``timeout``: Number.  The number of seconds to wait for a response before closing the connection for this request.
+
+  - Overrides the timeout value specified when the Redfish object is created for this request.
+  - This can be useful when a particular URI is known to take a long time to respond, such as with firmware updates.
+  - The default value is ``None``, which indicates the object-defined timeout is used.
+
+* ``max_retry``: Number.  The number of retries to perform an operation before giving up for this request.
+
+  - Overrides the max retry value specified when the Redfish object is created for this request.
+  - This can be useful when a particular URI is known to take multiple retries.
+  - The default value is ``None``, which indicates the object-defined max retry count is used.
+
 Working with tasks
 ~~~~~~~~~~~~~~~~~~
 
 POST, PATCH, PUT, and DELETE operations may result in a task, describing an operation with a duration greater than the span of a single request.
 The action message object that ``is_processing`` will return a task that can be accessed reviewed when polled with monitor.
 An example of a POST operation with a possible task is shown below.
```

### Comparing `redfish-3.2.0/src/redfish.egg-info/SOURCES.txt` & `redfish-3.2.1/src/redfish.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 src/redfish.egg-info/PKG-INFO
 src/redfish.egg-info/SOURCES.txt
 src/redfish.egg-info/dependency_links.txt
 src/redfish.egg-info/requires.txt
 src/redfish.egg-info/top_level.txt
 src/redfish/discovery/__init__.py
 src/redfish/discovery/discovery.py
+src/redfish/messages/__init__.py
+src/redfish/messages/messages.py
 src/redfish/rest/__init__.py
 src/redfish/rest/v1.py
 src/redfish/ris/__init__.py
 src/redfish/ris/config.py
 src/redfish/ris/ris.py
 src/redfish/ris/rmc.py
 src/redfish/ris/rmc_helper.py
```

