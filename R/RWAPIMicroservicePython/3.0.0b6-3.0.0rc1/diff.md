# Comparing `tmp/RWAPIMicroservicePython-3.0.0b6.tar.gz` & `tmp/RWAPIMicroservicePython-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWAPIMicroservicePython-3.0.0b6.tar", last modified: Fri Aug  4 08:20:48 2023, max compression
+gzip compressed data, was "RWAPIMicroservicePython-3.0.0rc1.tar", last modified: Fri Aug  4 09:55:57 2023, max compression
```

## Comparing `RWAPIMicroservicePython-3.0.0b6.tar` & `RWAPIMicroservicePython-3.0.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 08:20:48.652479 RWAPIMicroservicePython-3.0.0b6/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0b6/LICENSE
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-04 08:20:48.652479 RWAPIMicroservicePython-3.0.0b6/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2416 2023-08-03 13:11:16.000000 RWAPIMicroservicePython-3.0.0b6/README.md
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 08:20:48.652479 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/__init__.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/cloudwatch.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/errors.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     6554 2023-08-03 13:30:00.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/main.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2079 2023-08-03 13:19:32.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/test_utils.py
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 08:20:48.652479 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-04 08:20:48.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-04 08:20:48.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/SOURCES.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-04 08:20:48.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/dependency_links.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/not-zip-safe
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-04 08:20:48.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/requires.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-04 08:20:48.000000 RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython.egg-info/top_level.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-04 08:20:48.652479 RWAPIMicroservicePython-3.0.0b6/setup.cfg
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      888 2023-08-04 08:20:17.000000 RWAPIMicroservicePython-3.0.0b6/setup.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 09:55:57.182401 RWAPIMicroservicePython-3.0.0rc1/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0rc1/LICENSE
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 09:55:57.182401 RWAPIMicroservicePython-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     5996 2023-08-04 09:48:11.000000 RWAPIMicroservicePython-3.0.0rc1/README.md
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 09:55:57.179068 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/__init__.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/cloudwatch.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/errors.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     7055 2023-08-04 09:17:41.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/main.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2079 2023-08-03 13:19:32.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/test_utils.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-04 09:55:57.182401 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      365 2023-08-04 09:55:57.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-04 09:55:57.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-04 09:55:57.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/not-zip-safe
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-04 09:55:57.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/requires.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-04 09:55:57.000000 RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython.egg-info/top_level.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-04 09:55:57.182401 RWAPIMicroservicePython-3.0.0rc1/setup.cfg
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      886 2023-08-04 09:55:52.000000 RWAPIMicroservicePython-3.0.0rc1/setup.py
```

### Comparing `RWAPIMicroservicePython-3.0.0b6/LICENSE` & `RWAPIMicroservicePython-3.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/cloudwatch.py` & `RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/main.py` & `RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import requests
 import logging
-from flask import request, jsonify, Response
+from flask import request, jsonify, Response, Blueprint
 from requests import Session, Request
 from werkzeug.datastructures import ImmutableMultiDict
 
 from RWAPIMicroservicePython.errors import NotFound, ApiKeyError, ValidationError
 from RWAPIMicroservicePython.cloudwatch import CloudWatchService
 
 GATEWAY_URL: str = ''
@@ -24,38 +24,51 @@
 ):
     global MICROSERVICE_TOKEN, GATEWAY_URL
     MICROSERVICE_TOKEN = token
     GATEWAY_URL = gateway_url
 
     cloud_watch_service = CloudWatchService(aws_region, aws_cloud_watch_log_group_name, aws_cloud_watch_log_stream_name)
 
+    healthcheck_endpoint = Blueprint('rw_api_healthcheck', __name__)
+
+    @healthcheck_endpoint.route('/healthcheck', methods=['GET'])
+    def test_route():
+        return 'ok', 200
+
+    app.register_blueprint(healthcheck_endpoint)
+
     @app.after_request
     def set_cors_headers(response):
         response.headers["access-control-allow-origin"] = "*"
         response.headers["access-control-allow-headers"] = "upgrade-insecure-requests"
         response.headers["access-control-allow-credentials"] = "true"
         response.headers["access-control-allow-methods"] = "OPTIONS,GET,PUT,POST,PATCH,DELETE"
         return response
 
     @app.before_request
     def before_request():
+        if should_skip_api_key_validation():
+            return
         try:
             request_validation_data = get_logger_user()
         except ApiKeyError:
             return jsonify({'errors': {'message': 'Required API key not found', 'code': 403}}), 403
         except ValidationError as e:
             return Response(e.message, status=e.code, mimetype='application/json')
         except Exception as e:
             return e
 
         if aws_cloud_watch_logging_enabled:
             log_request_to_cloud_watch(request_validation_data)
 
         inject_request_validation_data(request_validation_data)
 
+    def should_skip_api_key_validation():
+        return request.path == '/healthcheck'
+
     def log_request_to_cloud_watch(request_validation_data):
         logging.debug('[log_request_to_cloud_watch] Logging request to CloudWatch')
 
         log_query = request.args.copy()
         if 'loggedUser' in log_query:
             del log_query['loggedUser']
         log_content = {
@@ -136,15 +149,16 @@
             )
 
             if logged_user_response.status_code >= 400:
                 raise ValidationError(message=logged_user_response.text, code=logged_user_response.status_code)
 
             json_response = logged_user_response.json()
 
-            if 'application' not in json_response and (json_response.get('user', {}).get('data', {}) .get('id', False) != 'microservice') and require_api_key:
+            if 'application' not in json_response and (json_response.get('user', {}).get('data', {}).get('id',
+                                                                                                         False) != 'microservice') and require_api_key:
                 raise ApiKeyError('Required API key not found')
 
             return json_response
         else:
             return {}
 
     @app.after_request
```

### Comparing `RWAPIMicroservicePython-3.0.0b6/RWAPIMicroservicePython/test_utils.py` & `RWAPIMicroservicePython-3.0.0rc1/RWAPIMicroservicePython/test_utils.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b6/setup.py` & `RWAPIMicroservicePython-3.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='RWAPIMicroservicePython',
-      version='3.0.0-beta.6',
+      version='3.0.0-rc.1',
       long_description='Python integration library for the RW API microservices',
       description='Python integration library for the RW API microservices',
       long_description_content_type='text',
       author='Vizzuality',
       author_email='info@vizzuality.com',
       url='https://vizzuality.com',
       license='MIT',
```

