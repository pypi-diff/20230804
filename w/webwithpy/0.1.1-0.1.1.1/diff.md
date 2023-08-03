# Comparing `tmp/webwithpy-0.1.1.tar.gz` & `tmp/webwithpy-0.1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.1.1.tar", max compression
+gzip compressed data, was "webwithpy-0.1.1.1.tar", max compression
```

## Comparing `webwithpy-0.1.1.tar` & `webwithpy-0.1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-31 21:55:53.778149 webwithpy-0.1.1/LICENSE
--rw-r--r--   0        0        0      100 2023-08-02 23:18:03.167190 webwithpy-0.1.1/README.md
--rw-r--r--   0        0        0      308 2023-08-03 22:46:48.603721 webwithpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 22:02:50.097559 webwithpy-0.1.1/webwithpy/__init__.py
--rw-r--r--   0        0        0      333 2023-08-02 23:04:12.980751 webwithpy-0.1.1/webwithpy/main.py
--rw-r--r--   0        0        0        0 2023-08-01 22:03:19.821707 webwithpy-0.1.1/webwithpy/wwp_data/__init__.py
--rw-r--r--   0        0        0      386 2023-07-31 22:01:00.125580 webwithpy-0.1.1/webwithpy/wwp_data/html_data.py
--rw-r--r--   0        0        0        0 2023-08-01 22:09:16.235517 webwithpy-0.1.1/webwithpy/wwp_handler/__init__.py
--rw-r--r--   0        0        0      774 2023-08-01 22:32:19.387018 webwithpy-0.1.1/webwithpy/wwp_handler/request_handlers.py
--rw-r--r--   0        0        0       36 2023-08-01 22:33:26.471649 webwithpy-0.1.1/webwithpy/wwp_requests/__init__.py
--rw-r--r--   0        0        0      770 2023-08-01 22:33:26.479649 webwithpy-0.1.1/webwithpy/wwp_requests/requests.py
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 webwithpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-31 21:55:53.778149 webwithpy-0.1.1.1/LICENSE
+-rw-r--r--   0        0        0      100 2023-08-02 23:18:03.167190 webwithpy-0.1.1.1/README.md
+-rw-r--r--   0        0        0      310 2023-08-03 22:56:02.588575 webwithpy-0.1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-08-03 22:54:00.084369 webwithpy-0.1.1.1/webwithpy/__init__.py
+-rw-r--r--   0        0        0      270 2023-08-03 22:53:49.680351 webwithpy-0.1.1.1/webwithpy/webwithpy.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:03:19.821707 webwithpy-0.1.1.1/webwithpy/wwp_data/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-31 22:01:00.125580 webwithpy-0.1.1.1/webwithpy/wwp_data/html_data.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:09:16.235517 webwithpy-0.1.1.1/webwithpy/wwp_handler/__init__.py
+-rw-r--r--   0        0        0      776 2023-08-03 22:54:26.780413 webwithpy-0.1.1.1/webwithpy/wwp_handler/request_handlers.py
+-rw-r--r--   0        0        0       36 2023-08-01 22:33:26.471649 webwithpy-0.1.1.1/webwithpy/wwp_requests/__init__.py
+-rw-r--r--   0        0        0      772 2023-08-03 22:54:11.584388 webwithpy-0.1.1.1/webwithpy/wwp_requests/requests.py
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 webwithpy-0.1.1.1/PKG-INFO
```

### Comparing `webwithpy-0.1.1/LICENSE` & `webwithpy-0.1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.1.1/webwithpy/wwp_handler/request_handlers.py` & `webwithpy-0.1.1.1/webwithpy/wwp_handler/request_handlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from http.server import BaseHTTPRequestHandler
-from wwp_data.html_data import HtmlData
+from ..wwp_data.html_data import HtmlData
 
 
 class HttpHandler(BaseHTTPRequestHandler):
     @classmethod
     def parse_http_handler_req(cls, handler, method):
         handler.send_response(200)
         handler.send_header('Content-type', 'text/html')
```

### Comparing `webwithpy-0.1.1/webwithpy/wwp_requests/requests.py` & `webwithpy-0.1.1.1/webwithpy/wwp_requests/requests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from wwp_data.html_data import HtmlData
+from ..wwp_data.html_data import HtmlData
 
 
 def generate_req_data_from_input(func, req_type: str, **kwargs) -> dict:
     combined_dict = {"func": func, "request_type": req_type}
     combined_dict.update(kwargs)
 
     return combined_dict
```

### Comparing `webwithpy-0.1.1/PKG-INFO` & `webwithpy-0.1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.1.1
+Version: 0.1.1.1
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

