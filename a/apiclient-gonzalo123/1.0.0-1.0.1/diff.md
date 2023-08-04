# Comparing `tmp/apiclient-gonzalo123-1.0.0.tar.gz` & `tmp/apiclient-gonzalo123-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiclient-gonzalo123-1.0.0.tar", last modified: Thu Aug  3 10:22:35 2023, max compression
+gzip compressed data, was "apiclient-gonzalo123-1.0.1.tar", last modified: Fri Aug  4 13:00:17 2023, max compression
```

## Comparing `apiclient-gonzalo123-1.0.0.tar` & `apiclient-gonzalo123-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-03 10:22:35.837934 apiclient-gonzalo123-1.0.0/
--rw-r--r--   0 gonzalo    (501) staff       (20)     1043 2023-08-03 10:22:35.837776 apiclient-gonzalo123-1.0.0/PKG-INFO
--rw-r--r--   0 gonzalo    (501) staff       (20)      608 2023-08-03 10:17:55.000000 apiclient-gonzalo123-1.0.0/README.md
-drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-03 10:22:35.836533 apiclient-gonzalo123-1.0.0/apiclient/
--rw-r--r--   0 gonzalo    (501) staff       (20)       52 2023-08-03 09:53:01.000000 apiclient-gonzalo123-1.0.0/apiclient/__init__.py
--rw-r--r--   0 gonzalo    (501) staff       (20)     1251 2023-08-03 09:58:23.000000 apiclient-gonzalo123-1.0.0/apiclient/apiclient.py
-drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-03 10:22:35.837561 apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/
--rw-r--r--   0 gonzalo    (501) staff       (20)     1043 2023-08-03 10:22:35.000000 apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/PKG-INFO
--rw-r--r--   0 gonzalo    (501) staff       (20)      282 2023-08-03 10:22:35.000000 apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/SOURCES.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)        1 2023-08-03 10:22:35.000000 apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/dependency_links.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)       16 2023-08-03 10:22:35.000000 apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/requires.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)       10 2023-08-03 10:22:35.000000 apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/top_level.txt
--rw-r--r--   0 gonzalo    (501) staff       (20)       38 2023-08-03 10:22:35.837969 apiclient-gonzalo123-1.0.0/setup.cfg
--rw-r--r--   0 gonzalo    (501) staff       (20)      816 2023-08-03 10:07:35.000000 apiclient-gonzalo123-1.0.0/setup.py
+drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-04 13:00:17.031298 apiclient-gonzalo123-1.0.1/
+-rw-r--r--   0 gonzalo    (501) staff       (20)     1045 2023-08-04 13:00:17.031103 apiclient-gonzalo123-1.0.1/PKG-INFO
+-rw-r--r--   0 gonzalo    (501) staff       (20)      610 2023-08-03 12:22:33.000000 apiclient-gonzalo123-1.0.1/README.md
+drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-04 13:00:17.029707 apiclient-gonzalo123-1.0.1/apiclient/
+-rw-r--r--   0 gonzalo    (501) staff       (20)       52 2023-08-03 09:53:01.000000 apiclient-gonzalo123-1.0.1/apiclient/__init__.py
+-rw-r--r--   0 gonzalo    (501) staff       (20)     1288 2023-08-04 12:58:12.000000 apiclient-gonzalo123-1.0.1/apiclient/apiclient.py
+drwxr-xr-x   0 gonzalo    (501) staff       (20)        0 2023-08-04 13:00:17.030868 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/
+-rw-r--r--   0 gonzalo    (501) staff       (20)     1045 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/PKG-INFO
+-rw-r--r--   0 gonzalo    (501) staff       (20)      282 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/SOURCES.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)        1 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/dependency_links.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)       16 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/requires.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)       10 2023-08-04 13:00:17.000000 apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/top_level.txt
+-rw-r--r--   0 gonzalo    (501) staff       (20)       38 2023-08-04 13:00:17.031338 apiclient-gonzalo123-1.0.1/setup.cfg
+-rw-r--r--   0 gonzalo    (501) staff       (20)      816 2023-08-04 12:58:24.000000 apiclient-gonzalo123-1.0.1/setup.py
```

### Comparing `apiclient-gonzalo123-1.0.0/PKG-INFO` & `apiclient-gonzalo123-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiclient-gonzalo123
-Version: 1.0.0
+Version: 1.0.1
 Summary: apiclient
 Home-page: https://github.com/gonzalo123/apiclient
 Author: Gonzalo Ayuso
 Author-email: gonzalo123@gmail.com
 License: MIT
 Keywords: apiclient
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 GET Request
 ```python
 data = client.get('/api/route', dict(param1='value1'))
 ```
 
 POST Request (with parameters in the url)
-```python
+```pythonº
 data = client.post('/api/route', params=dict(param1='value1'))
 ```
 
 POST Request (with parameters in the request body)
 ```python
 data = client.post('/api/route', body=dict(param1='value1'))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apiclient-gonzalo123-1.0.0/README.md` & `apiclient-gonzalo123-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 GET Request
 ```python
 data = client.get('/api/route', dict(param1='value1'))
 ```
 
 POST Request (with parameters in the url)
-```python
+```pythonº
 data = client.post('/api/route', params=dict(param1='value1'))
 ```
 
 POST Request (with parameters in the request body)
 ```python
 data = client.post('/api/route', body=dict(param1='value1'))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apiclient-gonzalo123-1.0.0/apiclient/apiclient.py` & `apiclient-gonzalo123-1.0.1/apiclient/apiclient.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     def _zip(columns, rows):
         return [dict(zip(columns, row)) for row in rows]
 
     @staticmethod
     def _get_headers(token):
         return {
             'token': token,
+            'x-client': 'apiclient',
             'Content-Type': 'application/json'
         }
 
     def _get_url(self, uri):
         return f'{self.base}{uri}'
 
     def _process_response(self, response):
```

### Comparing `apiclient-gonzalo123-1.0.0/apiclient_gonzalo123.egg-info/PKG-INFO` & `apiclient-gonzalo123-1.0.1/apiclient_gonzalo123.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiclient-gonzalo123
-Version: 1.0.0
+Version: 1.0.1
 Summary: apiclient
 Home-page: https://github.com/gonzalo123/apiclient
 Author: Gonzalo Ayuso
 Author-email: gonzalo123@gmail.com
 License: MIT
 Keywords: apiclient
 Classifier: Programming Language :: Python :: 3
@@ -34,15 +34,15 @@
 
 GET Request
 ```python
 data = client.get('/api/route', dict(param1='value1'))
 ```
 
 POST Request (with parameters in the url)
-```python
+```pythonº
 data = client.post('/api/route', params=dict(param1='value1'))
 ```
 
 POST Request (with parameters in the request body)
 ```python
 data = client.post('/api/route', body=dict(param1='value1'))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apiclient-gonzalo123-1.0.0/setup.py` & `apiclient-gonzalo123-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup_args = dict(
     name="apiclient-gonzalo123",
-    version="1.0.0",
+    version="1.0.1",
     author="Gonzalo Ayuso",
     author_email="gonzalo123@gmail.com",
     description="apiclient",
     long_description=long_description,
     license='MIT',
     long_description_content_type="text/markdown",
     keywords=['apiclient'],
```

