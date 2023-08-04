# Comparing `tmp/mbnk-0.2.1.tar.gz` & `tmp/mbnk-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.2.1.tar", max compression
+gzip compressed data, was "mbnk-0.4.0a0.tar", max compression
```

## Comparing `mbnk-0.2.1.tar` & `mbnk-0.4.0a0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1394 2023-07-05 20:55:27.254522 mbnk-0.2.1/README.md
--rw-r--r--   0        0        0      132 2023-07-05 20:55:27.254522 mbnk-0.2.1/mbnk/__init__.py
--rw-r--r--   0        0        0    21397 2023-07-05 22:20:52.459430 mbnk-0.2.1/mbnk/api.py
--rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.2.1/mbnk/asyncio/__init__.py
--rw-r--r--   0        0        0     1040 2023-07-05 20:55:27.254522 mbnk-0.2.1/mbnk/asyncio/mbnk.py
--rw-r--r--   0        0        0      576 2023-07-03 00:10:27.269164 mbnk-0.2.1/mbnk/exceptions.py
--rw-r--r--   0        0        0     1010 2023-07-05 20:55:27.254522 mbnk-0.2.1/mbnk/mbnk.py
--rw-r--r--   0        0        0      112 2023-07-05 20:55:27.254522 mbnk-0.2.1/mbnk/responses.py
--rw-r--r--   0        0        0     5286 2023-07-05 22:20:21.231145 mbnk-0.2.1/mbnk/types.py
--rw-r--r--   0        0        0       23 2023-07-02 22:21:13.141308 mbnk-0.2.1/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      603 2023-07-05 20:55:27.254522 mbnk-0.2.1/mbnk/utils/signature.py
--rw-r--r--   0        0        0      510 2023-07-02 22:21:26.081132 mbnk-0.2.1/mbnk/utils/webhook.py
--rw-r--r--   0        0        0      313 2023-07-05 22:21:36.987900 mbnk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1925 1970-01-01 00:00:00.000000 mbnk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1394 2023-07-05 20:55:27.254522 mbnk-0.4.0a0/README.md
+-rw-r--r--   0        0        0      132 2023-07-05 20:55:27.254522 mbnk-0.4.0a0/mbnk/__init__.py
+-rw-r--r--   0        0        0     7014 2023-07-30 10:51:50.041765 mbnk-0.4.0a0/mbnk/api.py
+-rw-r--r--   0        0        0      140 2023-07-03 20:40:21.439433 mbnk-0.4.0a0/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0     8704 2023-07-30 10:54:00.567087 mbnk-0.4.0a0/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     2856 2023-07-30 10:17:13.391876 mbnk-0.4.0a0/mbnk/enums.py
+-rw-r--r--   0        0        0      596 2023-07-12 12:34:28.846440 mbnk-0.4.0a0/mbnk/exceptions.py
+-rw-r--r--   0        0        0    11793 2023-07-30 10:50:58.712772 mbnk-0.4.0a0/mbnk/mbnk.py
+-rw-r--r--   0        0        0        0 2023-07-30 10:06:38.366881 mbnk-0.4.0a0/mbnk/methods/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-05 20:55:27.254522 mbnk-0.4.0a0/mbnk/responses.py
+-rw-r--r--   0        0        0     7358 2023-07-13 09:46:49.604104 mbnk-0.4.0a0/mbnk/types.py
+-rw-r--r--   0        0        0       48 2023-07-12 09:42:11.106776 mbnk-0.4.0a0/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      593 2023-07-30 10:07:56.175231 mbnk-0.4.0a0/mbnk/utils/signature.py
+-rw-r--r--   0        0        0      475 2023-07-30 09:54:51.371750 mbnk-0.4.0a0/mbnk/utils/webhook.py
+-rw-r--r--   0        0        0      411 2023-08-04 15:08:59.526799 mbnk-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 mbnk-0.4.0a0/PKG-INFO
```

### Comparing `mbnk-0.2.1/README.md` & `mbnk-0.4.0a0/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.2.1/mbnk/exceptions.py` & `mbnk-0.4.0a0/mbnk/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 #     'MonobankAPIException',
 #     'MonoPayAPIException'
 # ]
 
 from dataclasses import dataclass
 
 
-class MonobankOpenAPIException(Exception):
+class MonobankOpenAPIException(BaseException):
     error_description: str = ""
 
 
 class TooManyRequestsException(MonobankOpenAPIException):
     error_description: str = "MonobankException: Too many requests"
 
 
 @dataclass
-class MonobankAPIException:
+class MonobankAPIException(BaseException):
     err_description: str = None
 
 
 @dataclass
 class MonoPayAPIException:
     err_code: str = None
     err_text: str = None
     error_description: str = None
 
 
 class MonobankBadRequest(MonobankOpenAPIException):
     pass
+
```

### Comparing `mbnk-0.2.1/PKG-INFO` & `mbnk-0.4.0a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.2.1
-Summary: Sync/Async version monobank api
+Version: 0.4.0a0
+Summary: Sync/Async version Monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: ecdsa (>=0.18.0,<0.19.0)
+Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Mbnk
 <hr>
 
 ![PyPI](https://img.shields.io/pypi/v/mbnk)
```

