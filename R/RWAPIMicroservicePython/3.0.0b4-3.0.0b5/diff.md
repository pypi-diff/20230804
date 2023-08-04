# Comparing `tmp/RWAPIMicroservicePython-3.0.0b4.tar.gz` & `tmp/RWAPIMicroservicePython-3.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RWAPIMicroservicePython-3.0.0b4.tar", last modified: Thu Aug  3 09:32:18 2023, max compression
+gzip compressed data, was "RWAPIMicroservicePython-3.0.0b5.tar", last modified: Thu Aug  3 10:01:55 2023, max compression
```

## Comparing `RWAPIMicroservicePython-3.0.0b4.tar` & `RWAPIMicroservicePython-3.0.0b5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0b4/LICENSE
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2318 2023-07-31 11:34:02.000000 RWAPIMicroservicePython-3.0.0b4/README.md
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/__init__.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/cloudwatch.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/errors.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     6590 2023-08-01 14:44:13.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/main.py
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1943 2023-08-03 09:21:00.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/test_utils.py
-drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/PKG-INFO
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/SOURCES.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/dependency_links.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/not-zip-safe
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/requires.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-03 09:32:18.000000 RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython.egg-info/top_level.txt
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-03 09:32:18.140776 RWAPIMicroservicePython-3.0.0b4/setup.cfg
--rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      888 2023-08-03 09:31:54.000000 RWAPIMicroservicePython-3.0.0b4/setup.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 10:01:55.123891 RWAPIMicroservicePython-3.0.0b5/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     1100 2023-01-19 05:43:02.000000 RWAPIMicroservicePython-3.0.0b5/LICENSE
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 10:01:55.123891 RWAPIMicroservicePython-3.0.0b5/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2318 2023-07-31 11:34:02.000000 RWAPIMicroservicePython-3.0.0b5/README.md
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 10:01:55.123891 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      294 2023-08-03 09:29:42.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/__init__.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     3111 2023-08-01 12:50:17.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/cloudwatch.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      409 2023-07-31 16:10:42.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/errors.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     6590 2023-08-01 14:44:13.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/main.py
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)     2003 2023-08-03 09:57:00.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/test_utils.py
+drwxr-xr-x   0 tiagojsag  (1000) tiagojsag  (1000)        0 2023-08-03 10:01:55.123891 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      364 2023-08-03 10:01:55.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/PKG-INFO
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      484 2023-08-03 10:01:55.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/SOURCES.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-03 10:01:55.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/dependency_links.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)        1 2023-08-02 08:02:51.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/not-zip-safe
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      171 2023-08-03 10:01:55.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/requires.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       24 2023-08-03 10:01:55.000000 RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython.egg-info/top_level.txt
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)       38 2023-08-03 10:01:55.123891 RWAPIMicroservicePython-3.0.0b5/setup.cfg
+-rw-r--r--   0 tiagojsag  (1000) tiagojsag  (1000)      888 2023-08-03 10:01:44.000000 RWAPIMicroservicePython-3.0.0b5/setup.py
```

### Comparing `RWAPIMicroservicePython-3.0.0b4/LICENSE` & `RWAPIMicroservicePython-3.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b4/README.md` & `RWAPIMicroservicePython-3.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/cloudwatch.py` & `RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/main.py` & `RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/main.py`

 * *Files identical despite different names*

### Comparing `RWAPIMicroservicePython-3.0.0b4/RWAPIMicroservicePython/test_utils.py` & `RWAPIMicroservicePython-3.0.0b5/RWAPIMicroservicePython/test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -29,31 +29,31 @@
             "createdAt": "2023-06-28T15:00:48.149Z",
             "updatedAt": "2023-06-28T15:00:48.149Z"
         }
     }
 }
 
 
-def mock_request_validation(mocker, user=USER, application=APPLICATION['data']):
+def mock_request_validation(mocker, user=USER, application=APPLICATION['data'], microservice_token='microserviceToken'):
     response_json = {}
     if user is not None:
         response_json['user'] = {'data': user}
     if application is not None:
         response_json['application'] = {'data': application}
 
-    return mocker.post('http://gateway-url.com/v1/request/validate',
-                       request_headers={'Authorization': 'Bearer microserviceToken'},
+    return mocker.post('/v1/request/validate',
+                       request_headers={'Authorization': 'Bearer {}'.format(microservice_token)},
                        status_code=200,
                        json=response_json
                        )
 
 
-def mock_request_validation_invalid_token(mocker):
-    return mocker.post('http://gateway-url.com/v1/request/validate',
-                       request_headers={'Authorization': 'Bearer microserviceToken'},
+def mock_request_validation_invalid_token(mocker, microservice_token='microserviceToken'):
+    return mocker.post('/v1/request/validate',
+                       request_headers={'Authorization': 'Bearer {}'.format(microservice_token)},
                        status_code=401,
                        json={
                            "errors": [
                                {
                                    "status": 401,
                                    "detail": "Your token is outdated. Please use /auth/login to login and /auth/generate-token to generate a new token."
                                }
```

### Comparing `RWAPIMicroservicePython-3.0.0b4/setup.py` & `RWAPIMicroservicePython-3.0.0b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 setup(name='RWAPIMicroservicePython',
-      version='3.0.0-beta.4',
+      version='3.0.0-beta.5',
       long_description='Python integration library for the RW API microservices',
       description='Python integration library for the RW API microservices',
       long_description_content_type='text',
       author='Vizzuality',
       author_email='info@vizzuality.com',
       url='https://vizzuality.com',
       license='MIT',
```

