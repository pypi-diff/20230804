# Comparing `tmp/wiliot-api-4.3.2.tar.gz` & `tmp/wiliot-api-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-api-4.3.2.tar", last modified: Thu Jul 20 02:41:00 2023, max compression
+gzip compressed data, was "wiliot-api-4.4.0.tar", last modified: Fri Aug  4 07:56:13 2023, max compression
```

## Comparing `wiliot-api-4.3.2.tar` & `wiliot-api-4.4.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4217 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3711 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)     9514 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      328 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1685 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/
--rw-rw-rw-   0 root         (0) root         (0)     4293 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11463 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/api_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/edge/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/edge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15717 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/edge/edge.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/edge/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/edge/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5799 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/edge/examples/edge_api.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/manufacturing/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/manufacturing/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/manufacturing/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/manufacturing/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5327 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/manufacturing/examples/mannufacturing_api.py
--rw-rw-rw-   0 root         (0) root         (0)    14099 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/manufacturing/manufacturing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/platform/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/platform/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/platform/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/platform/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5899 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/platform/examples/platform_api.py
--rw-rw-rw-   0 root         (0) root         (0)    35971 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/platform/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3075 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/platform/platform_models.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/security/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/security/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7223 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/security/security.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6184 2023-07-20 02:40:43.000000 wiliot-api-4.3.2/wiliot_api/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-20 02:41:00.306806 wiliot-api-4.3.2/wiliot_api.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4217 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2023-07-20 02:41:00.000000 wiliot-api-4.3.2/wiliot_api.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4452 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9514 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      328 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.310261 wiliot-api-4.4.0/wiliot_api/
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11676 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/api_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.310261 wiliot-api-4.4.0/wiliot_api/edge/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/edge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15774 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/edge/edge.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.310261 wiliot-api-4.4.0/wiliot_api/edge/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/edge/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5799 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/edge/examples/edge_api.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/wiliot_api/manufacturing/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/manufacturing/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/wiliot_api/manufacturing/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/manufacturing/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5327 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/manufacturing/examples/mannufacturing_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    14099 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/manufacturing/manufacturing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/wiliot_api/platform/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/platform/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/wiliot_api/platform/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/platform/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5899 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/platform/examples/platform_api.py
+-rw-rw-rw-   0 root         (0) root         (0)    35999 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/platform/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3075 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/platform/platform_models.py
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/wiliot_api/security/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/security/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7096 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/security/security.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.314261 wiliot-api-4.4.0/wiliot_api/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6184 2023-08-04 07:55:56.000000 wiliot-api-4.4.0/wiliot_api/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-04 07:56:13.310261 wiliot-api-4.4.0/wiliot_api.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4452 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-08-04 07:56:13.000000 wiliot-api-4.4.0/wiliot_api.egg-info/top_level.txt
```

### Comparing `wiliot-api-4.3.2/LICENSE` & `wiliot-api-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/PKG-INFO` & `wiliot-api-4.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.3.2
+Version: 4.4.0
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,20 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.4.0:
+-----------------
+* Forcing a token refresh when an access token is less than a minute from expiry
+* Added support for alternate clouds and regions
+* Streamlined API paths to match between the platform and edge modules
+
 Version 4.3.2:
 -----------------
 * Added an option to get a binary file from the API
 * Added a function for sending actions to a gateway
 
 Version 4.3.1:
 -----------------
```

### Comparing `wiliot-api-4.3.2/README.md` & `wiliot-api-4.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,20 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.4.0:
+-----------------
+* Forcing a token refresh when an access token is less than a minute from expiry
+* Added support for alternate clouds and regions
+* Streamlined API paths to match between the platform and edge modules
+
 Version 4.3.2:
 -----------------
 * Added an option to get a binary file from the API
 * Added a function for sending actions to a gateway
 
 Version 4.3.1:
 -----------------
```

### Comparing `wiliot-api-4.3.2/bitbucket-pipelines.yml` & `wiliot-api-4.4.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/setup.py` & `wiliot-api-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/__init__.py` & `wiliot-api-4.4.0/wiliot_api/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/api_client.py` & `wiliot-api-4.4.0/wiliot_api/api_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,26 +68,32 @@
 
 class WiliotCloudError(Exception):
     pass
 
 
 class Client:
     def __init__(self, oauth_username=None, oauth_password=None, api_key=None,
-                 env='prod', api_version='v1', log_file=None, logger_=None):
+                 env='prod', api_version='v1', region='us-east-2', cloud='', log_file=None, logger_=None):
         # The caller must provide either a set of oauth username abd password or an API key
         if api_key is None and (oauth_password is None or oauth_username is None):
             raise Exception('Provide either an API key or a username and password')
         
-        self.env = env
+        self.env = env if env != '' else 'prod'
         self.api_version = api_version
+        self.region = region
+        if cloud != '':
+            self.cloud = "."+cloud
+        else:
+            self.cloud = ""
+        self.base_path = f"https://api.{region}.{self.env}{self.cloud}.wiliot.cloud/"
         self.headers = {
             "accept": "application/json",
             "Content-Type": "application/json"
         }
-        self.auth_obj = security.WiliotAuthentication(base_path=f"https://api.us-east-2.{self.env}.wiliot.cloud/{self.api_version}/",
+        self.auth_obj = security.WiliotAuthentication(base_path=f"{self.base_path}/{self.api_version}/",
                                                       oauth_username=oauth_username,
                                                       oauth_password=oauth_password,
                                                       api_key=api_key)
         self.headers["Authorization"] = self.auth_obj.get_token()
         if logger_ is None:
             self.logger = logging.getLogger()
             self.logger.setLevel(log_level)
@@ -101,15 +107,15 @@
                 self.handler = logging.StreamHandler()
             self.handler.setLevel(log_level)
             formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
             self.handler.setFormatter(formatter)
             self.logger.addHandler(self.handler)
 
     def _get_base_url(self, override_client_path=None, override_api_version=None):
-        api_path = f"https://api.us-east-2.{self.env}.wiliot.cloud/{self.api_version if override_api_version is None else override_api_version}/"
+        api_path = f"{self.base_path}/{self.api_version if override_api_version is None else override_api_version}/"
         base_url = api_path + self.client_path if override_client_path is None else api_path + override_client_path
         return base_url
 
     def _renew_token(self):
         if self.auth_obj.token_expired():
             self.headers["Authorization"] = self.auth_obj.get_token()
```

### Comparing `wiliot-api-4.3.2/wiliot_api/edge/edge.py` & `wiliot-api-4.4.0/wiliot_api/edge/edge.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,18 +71,18 @@
 
 class BridgeAction(Enum):
     BLINK_LED = 'blinkBridgeLed'
     REBOOT = 'rebootBridge'
 
 
 class EdgeClient(Client):
-    def __init__(self, api_key, owner_id, env='prod', log_file=None, logger_=None):
+    def __init__(self, api_key, owner_id, env='prod', region='us-east-2', cloud='',log_file=None, logger_=None):
         self.client_path = f"owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
-        super().__init__(api_key=api_key, env=env, log_file=log_file, logger_=logger_)
+        super().__init__(api_key=api_key, env=env, region=region, cloud=cloud, log_file=log_file, logger_=logger_)
 
     def get_gateways(self):
         """
         Get a list of gateways owned by the owner
         :return: A list of gateways
         """
         path = "gateway"
```

### Comparing `wiliot-api-4.3.2/wiliot_api/edge/examples/edge_api.py` & `wiliot-api-4.4.0/wiliot_api/edge/examples/edge_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/manufacturing/examples/mannufacturing_api.py` & `wiliot-api-4.4.0/wiliot_api/manufacturing/examples/mannufacturing_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/manufacturing/manufacturing.py` & `wiliot-api-4.4.0/wiliot_api/manufacturing/manufacturing.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/platform/examples/platform_api.py` & `wiliot-api-4.4.0/wiliot_api/platform/examples/platform_api.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/platform/platform.py` & `wiliot-api-4.4.0/wiliot_api/platform/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,18 +104,18 @@
 
 
 class LocationAssociationType(Enum):
     BRIDGE = 'bridge'
 
 
 class PlatformClient(Client):
-    def __init__(self, api_key, owner_id, env='prod', log_file=None, logger_=None):
+    def __init__(self, api_key, owner_id, env='prod', region='us-east-2', cloud='', log_file=None, logger_=None):
         self.client_path = "traceability/owner/{owner_id}/".format(owner_id=owner_id)
         self.owner_id = owner_id
-        super().__init__(api_key=api_key, env=env, log_file=log_file, logger_=logger_)
+        super().__init__(api_key=api_key, env=env, region=region, cloud=cloud, log_file=log_file, logger_=logger_)
 
     # Tag calls
 
     def get_pixels(self, limit=None, next=None):
         """
         Get an owner's pixels
         :param limit: Optional integer - limit the number of pixels to return (default: 50)
@@ -133,15 +133,15 @@
     # Asset calls
 
     def get_assets(self):
         """
         Get all assets or a subset of assets
         :return: A list of asset dictionaries
         """
-        path = "/metadataFetch"
+        path = "metadataFetch"
 
         has_next = True
         cursor = None
         assets = []
         from .platform_models import Query, Operation, StringFilter
 
         while True:
@@ -183,15 +183,15 @@
         """
         Get a single assets for a project
         :param asset_id: string
         :return: a dictionary with asset properties
         :raises: An AssetNotFound exception if an asset with the
         provided ID cannot be found
         """
-        path = "/metadataFetch"
+        path = "metadataFetch"
 
         from .platform_models import Query, Operation, StringFilter
 
         query = Operation(Query)
         query.assets(id={'filterType': 'equalTo', 'value': asset_id})
         # query.assets.page.__fields__()
         # Define the fields to return
@@ -232,15 +232,15 @@
          > tagId: string
          > role: Enum: TagRole
         :param asset_id: String - optional. If not provided an asset ID will be generated automatically
         :param status: String - optional - A status
         :return: The created asset if successful
         """
         assert isinstance(pixels, list), "Expecting a list of strings for pixels_ids"
-        path = "/asset"
+        path = "asset"
         payload = {
             "id": asset_id,
             "name": name,
             "categoryId": category_id,
             "tags": [{
                 'tagId': t['tagId'],
                 'role': t['role'].value
@@ -258,15 +258,15 @@
         """
         Update an asset. The following asset properties can be updated:
         * Category
         * Name
         :param asset: Dictionary describing the new asset properties
         :return: The updated asset if successful
         """
-        path = "/asset/{}".format(asset["id"])
+        path = "asset/{}".format(asset["id"])
         payload = {
             "name": asset.get("name", None),
             "categoryId": asset.get("categoryId", None),
             "status": asset.get("status", None)
         }
         try:
             res = self._put(path, payload, override_api_version="v2")
@@ -277,15 +277,15 @@
 
     def delete_asset(self, asset_id):
         """
         Delete an asset by its ID
         :param asset_id: String - required - the ID of the asset to delete
         :return: True if the asset was deleted
         """
-        path = "/asset/{}".format(asset_id)
+        path = "asset/{}".format(asset_id)
         try:
             res = self._delete(path, override_api_version="v2")
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete asset")
             raise e
         
@@ -382,15 +382,15 @@
     # Category calls
 
     def get_categories(self):
         """
         Get all asset categories
         :return: a list of dictionaries with categories
         """
-        path = "/metadataFetch"
+        path = "metadataFetch"
 
         has_next = True
         cursor = None
         categories = []
         from .platform_models import Query, Operation, StringFilter
 
         while True:
@@ -417,15 +417,15 @@
         """
         Get a single asset type for a project
         :param category_id: string
         :return: a dictionary with asset type properties
         :raises: An AssetTypeNotFound exception if an asset with the
         provided ID cannot be found
         """
-        path = "/asset/type/{}".format(category_id)
+        path = "asset/type/{}".format(category_id)
         res = self._get(path)
         if len(res.get('data', [])) == 0:
             raise CategoryNotFound
         return res.get('data', [])
 
     def create_category(self, name, asset_type_id, events, category_id=None, sku=None, description=None):
         """
@@ -437,15 +437,15 @@
         :param category_id: String - optional - If not provided an asset ID will be generated automatically
         :param sku: String - optional - A SKU/UPC to link the category to
         :param description: String - optional - A description for the category
         :return: The created asset if successful
         """
         # Make sure events is a list of Events
         assert isinstance(events, list) and all(isinstance(element, Event) for element in events), "events argument must be a list of Event(s)"
-        path = "/category"
+        path = "category"
         payload = {
             "assetType": {
                 "events": [
                     {
                         "selected": True,
                         "eventName": e.value
                     } for e in events
@@ -466,54 +466,54 @@
 
     def update_category(self, category):
         """
         Update a category
         :param category: Dictionary describing the category
         :return: The updated category if successful
         """
-        path = "/asset/type/{}".format(category['id'])
+        path = "asset/type/{}".format(category['id'])
         try:
             res = self._put(path, category)
             return res['data']
         except WiliotCloudError as e:
             print("Failed to update asset type")
             raise e
 
     def delete_category(self, category_id):
         """
         Delete a category by its ID
         :param category_id: String - required - the ID of the category to delete
         :return: True if the asset was deleted
         """
-        path = "/category/{}".format(category_id)
+        path = "category/{}".format(category_id)
         try:
             res = self._delete(path)
             print(res['message'])
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete category")
             raise e
 
     # Asset types
     def get_asset_types(self):
         """
         Get all asset types
         :return: a list of dictionaries with asset types
         """
-        path = "/asset-type"
+        path = "asset-type"
         res = self._get(path)
         return res.get('data', [])
 
     # Locations
     def get_locations(self):
         """
         Get all locations
         :return: A list of dictionaries representing locations
         """
-        path = "/metadataFetch"
+        path = "metadataFetch"
 
         has_next = True
         cursor = None
         locations = []
         from .platform_models import Query, Operation, StringFilter
 
         while True:
@@ -539,15 +539,15 @@
     def get_location(self, location_id):
         """
         Get one location
         :param location_id: String - required - the ID of the location to return
         :return: A dictionary representing the location
         :raise: A LocationNotFound if a location with the provided ID does not exist
         """
-        path = f"/location/{location_id}"
+        path = f"location/{location_id}"
         res = self._get(path)
         if len(res.get('data', [])) == 0:
             raise LocationNotFound
         return res.get('data', [])
 
     def create_location(self, location_type, name=None, location_id=None, lat=None, lng=None,
                         address=None, city=None, country=None):
@@ -560,15 +560,15 @@
         :param lat: Float - Optional - The latitude value for the location - required only for location type SITE
         :param lng: Float - Optional - The longitude value for the location - required only for location type SITE
         :param address: String - Optional - A street address for the location
         :param city: String - Optional - The location's city
         :param country: String - Optional - the location's country
         :return: The created location if successful
         """
-        path = "/location"
+        path = "location"
         payload = {
             'locationType': location_type.value,
             'id': location_id,
             'name': name,
             'lat': lat,
             'lng': lng,
             'address': address,
@@ -586,15 +586,15 @@
         """
         Update a location
         :param location: Dictionary - Required - The updated location dictionary. All location properties, except for
         location ID can be updated
         :return: The updated location if successful
         :raise: LocationNotFound if the requested location does not exit
         """
-        path = f"/location/{location['id']}"
+        path = f"location/{location['id']}"
         payload = {
             'locationType': location['locationType'].value if isinstance(location, LocationType) else location['locationType'],
             'name': location.get('name', None),
             'lat': location.get('lat', None),
             'lng': location.get('lng', None),
             'address': location.get('address', None),
             'city': location.get('city', None),
@@ -609,30 +609,30 @@
 
     def delete_location(self, location_id):
         """
         Delete a location
         :param location_id: String - Required - The ID of the location to delete
         :return: True if the location was deleted
         """
-        path = f"/location/{location_id}"
+        path = f"location/{location_id}"
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete location")
             raise e
 
     # Associations
     def get_location_associations(self, location_id):
         """
         Get all associations for a given location
         :param location_id: String - Required - The location ID to return associations for
         :return: A list of associations
         """
-        path = "/fetchMetadata"
+        path = "fetchMetadata"
 
         has_next = True
         cursor = None
         poi_associations = []
         from .platform_models import Query, Operation, StringFilter
 
         while True:
@@ -660,15 +660,15 @@
         Create a new association for a location
         :param location_id: String - Required - The ID of the location to create the association for
         :param association_type: LocationAssociationType - Required - The type of association
         :param association_value: String - Required - The value of the association (the bridge ID in case of a bridge
          association)
         :return: The new association that was created
         """
-        path = f"/location/{location_id}/association"
+        path = f"location/{location_id}/association"
         payload = {
             'associationValue': association_value,
             'associationType': association_type.value
         }
         try:
             res = self._post(path, payload=payload)
             return res['data']
@@ -680,45 +680,45 @@
         """
         Delete one location association
         :param location_id: String - Required - The ID of the location to delete associations for
         :param association_value: String - Required - Provide a value to delete only one association
         value.
         :return: True if successful
         """
-        path = f"/location/{location_id}/association/{association_value}"
+        path = f"location/{location_id}/association/{association_value}"
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete a location association")
             raise e
 
     def delete_location_associations(self, location_id):
         """
         Delete all location associations
         :param location_id: String - Required - The ID of the location to delete associations for
         value.
         :return: True if successful
         """
-        path = f"/location/{location_id}/association"
+        path = f"location/{location_id}/association"
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete location associations")
             raise e
 
     def get_zone_associations(self, zone_id):
         """
         Get all associations for a given zone
         :param location_id: String - Required - The location ID the zone belongs to
         :param zone_id: String - Required - The zone ID to query
         :return: A list of associations
         """
-        path = "/fetchMetadata"
+        path = "fetchMetadata"
 
         has_next = True
         cursor = None
         poi_associations = []
         from .platform_models import Query, Operation, StringFilter
 
         while True:
@@ -746,15 +746,15 @@
         Create a new association for a location
         :param location_id: String - Required - The ID of the location to create the association for
         :param zone_id: String - Required -  The ID of the zone to create the association for
         :param association_type: ZoneAssociationType - Required - The type of association
         :param association_value: String - Required - The value of the association (bridge ID in case of bridge)
         :return: The new association that was created
         """
-        path = f"/location/{location_id}/zone/{zone_id}/association"
+        path = f"location/{location_id}/zone/{zone_id}/association"
         payload = {
             'associationValue': association_value,
             'associationType': association_type.value
         }
         try:
             res = self._post(path, payload=payload)
             return res['data']
@@ -767,44 +767,44 @@
         Delete one zone association
         :param location_id: String - Required - The ID of the location the zone belongs to
         :param zone_id: String - Required - The ID of the zone to delete the association from
         :param association_value: String - Required - Provide a value to delete only one association
         value.
         :return: True if successful
         """
-        path = f"/location/{location_id}/zone/{zone_id}/association/{association_value}"
+        path = f"location/{location_id}/zone/{zone_id}/association/{association_value}"
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete a zone association")
             raise e
 
     def delete_zone_associations(self, location_id, zone_id):
         """
         Delete all zone associations
         :param location_id: String - Required - The ID of the location the zone belongs to
         :param zone_id: String - Required - The ID of the zone to delete the associations from
         :return: True if successful
         """
-        path = f"/location/{location_id}/zone/{zone_id}/association"
+        path = f"location/{location_id}/zone/{zone_id}/association"
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete zone associations")
 
     # Zones
     def get_zones(self, location_id=None):
         """
         Get all zones (can be filtered by location)
         :param location_id: The ID of the location to return zones belonging to
         :return: A list of zones
         """
-        path = "/fetchMetdata"
+        path = "fetchMetdata"
 
         has_next = True
         cursor = None
         zones = []
         from .platform_models import Query, Operation, StringFilter
 
         while True:
@@ -837,30 +837,30 @@
         """
         Get all zones under a location
         :param location_id: The ID of the location the zone belongs to
         :param zone_id: The ID of the zone to return
         :return: A list of zones
         :raise: A ZoneNotFound exception if a zone with the requested ID does not exist
         """
-        path = f"/location/{location_id}/zone/{zone_id}"
+        path = f"location/{location_id}/zone/{zone_id}"
         res = self._get(path)
         if len(res.get('data', [])) == 0:
             raise ZoneNotFound
         return res.get('data', [])
 
     def create_zone(self, name, location_id, zone_id=None):
         """
         Create a new zone
         :param name: String - Required - A human-readable name for the zone
         :param location_id: String - Required - The ID the zone will belong to
         :param zone_id: String - optional - The ID to give to the zone.
         If none is provided an ID will be automatically generated
         :return: The created zone
         """
-        path = f"/location/{location_id}/zone"
+        path = f"location/{location_id}/zone"
         payload = {
             'name': name,
             'id': zone_id
         }
         try:
             res = self._post(path, payload)
             return res['data']
@@ -872,15 +872,15 @@
         """
         Update a zone
         :param location_id: String - Required - The ID of the location the zone belongs to
         :param zone: Dictionary - Required - The updated zone dictionary. All location properties, except for
         zone ID can be updated
         :return: The updated zone if successful
         """
-        path = f"/location/{location_id}/zone/{zone['id']}"
+        path = f"location/{location_id}/zone/{zone['id']}"
         payload = {
             'name': zone['name'],
             'id': zone['id'],
             'locationId': zone['locationId']
         }
         try:
             res = self._put(path, payload)
@@ -892,28 +892,28 @@
     def delete_zone(self, location_id, zone_id):
         """
         Delete a zone
         :param location_id: String - Required - The ID of the location the zone belongs to
         :param zone_id: String - Required - The ID of the location to delete
         :return: True if the location was deleted
         """
-        path = f"/location/{location_id}/zone/{zone_id}"
+        path = f"location/{location_id}/zone/{zone_id}"
         try:
             res = self._delete(path)
             return res['message'].lower().find("success") != -1
         except WiliotCloudError as e:
             print("Failed to delete zone")
             raise e
 
     def query_metadata(self,  query):
         """
         Execute a query to get metadata
         :param query: String - Required - The query to send
         """
-        path = f"/metadataFetch"
+        path = f"metadataFetch"
         payload = {
             "query": query
         }
         try:
             res = self._post(path, payload)
             return res["data"]
         except WiliotCloudError as e:
```

### Comparing `wiliot-api-4.3.2/wiliot_api/platform/platform_models.py` & `wiliot-api-4.4.0/wiliot_api/platform/platform_models.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api/security/security.py` & `wiliot-api-4.4.0/wiliot_api/security/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,20 +131,18 @@
                 else:
                     raise e
         elif self.api_key is not None:
             auth_res = self._get_token_from_server_with_api_key()
         return auth_res
     
     def get_token(self):
-        if self.token is None or self.token["expires_on"] < datetime.now() - timedelta(
-                seconds=self.min_token_duration):
-            self.token = self._get_token_from_server()
-            # Add an "expires_on" field to reflect the date and this token will expire
-            self.token["expires_on"] = datetime.now() + timedelta(seconds=self.token["expires_in"])
+        self.token = self._get_token_from_server()
+        # Add an "expires_on" field to reflect the date and this token will expire
+        self.token["expires_on"] = datetime.now() + timedelta(seconds=self.token["expires_in"])
         
         return self.token["access_token"]
     
     def token_expired(self):
-        return self.token is None or self.token["expires_on"] < datetime.now()
+        return self.token is None or self.token["expires_on"] < datetime.now() + timedelta(minutes=1)
     
     def set_min_token_duration(self, min_token_duration):
         self.min_token_duration = min_token_duration
```

### Comparing `wiliot-api-4.3.2/wiliot_api/utils/get_version.py` & `wiliot-api-4.4.0/wiliot_api/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-api-4.3.2/wiliot_api.egg-info/PKG-INFO` & `wiliot-api-4.4.0/wiliot_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-api
-Version: 4.3.2
+Version: 4.4.0
 Summary: A library for interacting with Wiliot's private Cloud API
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -57,14 +57,20 @@
 * [platform](wiliot_api/platform/examples)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
 
+Version 4.4.0:
+-----------------
+* Forcing a token refresh when an access token is less than a minute from expiry
+* Added support for alternate clouds and regions
+* Streamlined API paths to match between the platform and edge modules
+
 Version 4.3.2:
 -----------------
 * Added an option to get a binary file from the API
 * Added a function for sending actions to a gateway
 
 Version 4.3.1:
 -----------------
```

### Comparing `wiliot-api-4.3.2/wiliot_api.egg-info/SOURCES.txt` & `wiliot-api-4.4.0/wiliot_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

