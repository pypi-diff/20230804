# Comparing `tmp/webwithpy-0.1.0.tar.gz` & `tmp/webwithpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webwithpy-0.1.0.tar", max compression
+gzip compressed data, was "webwithpy-0.1.1.tar", max compression
```

## Comparing `webwithpy-0.1.0.tar` & `webwithpy-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-31 21:55:53.778149 webwithpy-0.1.0/LICENSE
--rw-r--r--   0        0        0      100 2023-08-02 23:18:03.167190 webwithpy-0.1.0/README.md
--rw-r--r--   0        0        0      283 2023-08-02 23:18:16.043206 webwithpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 22:02:50.097559 webwithpy-0.1.0/webwithpy/__init__.py
--rw-r--r--   0        0        0      333 2023-08-02 23:04:12.980751 webwithpy-0.1.0/webwithpy/main.py
--rw-r--r--   0        0        0        0 2023-08-01 22:03:19.821707 webwithpy-0.1.0/webwithpy/wwp_data/__init__.py
--rw-r--r--   0        0        0      142 2023-08-01 22:04:46.574142 webwithpy-0.1.0/webwithpy/wwp_data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      587 2023-08-01 22:04:46.574142 webwithpy-0.1.0/webwithpy/wwp_data/__pycache__/html_data.cpython-310.pyc
--rw-r--r--   0        0        0      386 2023-07-31 22:01:00.125580 webwithpy-0.1.0/webwithpy/wwp_data/html_data.py
--rw-r--r--   0        0        0        0 2023-08-01 22:09:16.235517 webwithpy-0.1.0/webwithpy/wwp_handler/__init__.py
--rw-r--r--   0        0        0      149 2023-08-01 22:11:48.560305 webwithpy-0.1.0/webwithpy/wwp_handler/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1141 2023-08-01 22:32:27.047164 webwithpy-0.1.0/webwithpy/wwp_handler/__pycache__/request_handlers.cpython-310.pyc
--rw-r--r--   0        0        0      774 2023-08-01 22:32:19.387018 webwithpy-0.1.0/webwithpy/wwp_handler/request_handlers.py
--rw-r--r--   0        0        0       36 2023-08-01 22:33:26.471649 webwithpy-0.1.0/webwithpy/wwp_requests/__init__.py
--rw-r--r--   0        0        0      215 2023-08-01 22:33:47.343774 webwithpy-0.1.0/webwithpy/wwp_requests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-08-01 22:33:47.343774 webwithpy-0.1.0/webwithpy/wwp_requests/__pycache__/requests.cpython-310.pyc
--rw-r--r--   0        0        0      770 2023-08-01 22:33:26.479649 webwithpy-0.1.0/webwithpy/wwp_requests/requests.py
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 webwithpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-31 21:55:53.778149 webwithpy-0.1.1/LICENSE
+-rw-r--r--   0        0        0      100 2023-08-02 23:18:03.167190 webwithpy-0.1.1/README.md
+-rw-r--r--   0        0        0      308 2023-08-03 22:46:48.603721 webwithpy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 22:02:50.097559 webwithpy-0.1.1/webwithpy/__init__.py
+-rw-r--r--   0        0        0      333 2023-08-02 23:04:12.980751 webwithpy-0.1.1/webwithpy/main.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:03:19.821707 webwithpy-0.1.1/webwithpy/wwp_data/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-31 22:01:00.125580 webwithpy-0.1.1/webwithpy/wwp_data/html_data.py
+-rw-r--r--   0        0        0        0 2023-08-01 22:09:16.235517 webwithpy-0.1.1/webwithpy/wwp_handler/__init__.py
+-rw-r--r--   0        0        0      774 2023-08-01 22:32:19.387018 webwithpy-0.1.1/webwithpy/wwp_handler/request_handlers.py
+-rw-r--r--   0        0        0       36 2023-08-01 22:33:26.471649 webwithpy-0.1.1/webwithpy/wwp_requests/__init__.py
+-rw-r--r--   0        0        0      770 2023-08-01 22:33:26.479649 webwithpy-0.1.1/webwithpy/wwp_requests/requests.py
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 webwithpy-0.1.1/PKG-INFO
```

### Comparing `webwithpy-0.1.0/LICENSE` & `webwithpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webwithpy-0.1.0/webwithpy/wwp_handler/request_handlers.py` & `webwithpy-0.1.1/webwithpy/wwp_handler/request_handlers.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.1.0/webwithpy/wwp_requests/requests.py` & `webwithpy-0.1.1/webwithpy/wwp_requests/requests.py`

 * *Files identical despite different names*

### Comparing `webwithpy-0.1.0/PKG-INFO` & `webwithpy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webwithpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Sven Keimpema
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

