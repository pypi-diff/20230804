# Comparing `tmp/py-ke-utils-fastapi-2.0.2.tar.gz` & `tmp/py-ke-utils-fastapi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ke-utils-fastapi-2.0.2.tar", last modified: Thu Jun 29 12:32:31 2023, max compression
+gzip compressed data, was "py-ke-utils-fastapi-2.1.0.tar", last modified: Fri Aug  4 09:28:41 2023, max compression
```

## Comparing `py-ke-utils-fastapi-2.0.2.tar` & `py-ke-utils-fastapi-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 12:32:31.118664 py-ke-utils-fastapi-2.0.2/
--rw-r--r--   0 erne      (1000) erne      (1000)      499 2023-06-29 12:32:31.118664 py-ke-utils-fastapi-2.0.2/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)     6383 2023-06-28 13:12:43.000000 py-ke-utils-fastapi-2.0.2/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 12:32:31.118664 py-ke-utils-fastapi-2.0.2/py_ke_utils_fastapi.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      499 2023-06-29 12:32:30.000000 py-ke-utils-fastapi-2.0.2/py_ke_utils_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      292 2023-06-29 12:32:30.000000 py-ke-utils-fastapi-2.0.2/py_ke_utils_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 12:32:30.000000 py-ke-utils-fastapi-2.0.2/py_ke_utils_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       42 2023-06-29 12:32:30.000000 py-ke-utils-fastapi-2.0.2/py_ke_utils_fastapi.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-06-29 12:32:30.000000 py-ke-utils-fastapi-2.0.2/py_ke_utils_fastapi.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 12:32:31.118664 py-ke-utils-fastapi-2.0.2/pykeutilsfastapi/
--rw-r--r--   0 erne      (1000) erne      (1000)       47 2023-06-29 12:25:20.000000 py-ke-utils-fastapi-2.0.2/pykeutilsfastapi/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     5159 2023-06-29 12:31:59.000000 py-ke-utils-fastapi-2.0.2/pykeutilsfastapi/_auth_deco.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 12:32:31.118664 py-ke-utils-fastapi-2.0.2/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      772 2023-06-29 12:32:13.000000 py-ke-utils-fastapi-2.0.2/setup.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/PKG-INFO
+-rwxrwxrwx   0 vgurin    (1000) vgurin    (1000)     6383 2023-04-11 16:05:08.000000 py-ke-utils-fastapi-2.1.0/README.md
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/py_ke_utils_fastapi.egg-info/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      424 2023-08-04 09:28:41.000000 py-ke-utils-fastapi-2.1.0/py_ke_utils_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      415 2023-08-04 09:28:41.000000 py-ke-utils-fastapi-2.1.0/py_ke_utils_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        1 2023-08-04 09:28:41.000000 py-ke-utils-fastapi-2.1.0/py_ke_utils_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       43 2023-08-04 09:28:41.000000 py-ke-utils-fastapi-2.1.0/py_ke_utils_fastapi.egg-info/requires.txt
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       17 2023-08-04 09:28:41.000000 py-ke-utils-fastapi-2.1.0/py_ke_utils_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:13:01.000000 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/__init__.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/keycloak/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       76 2023-08-04 09:28:32.000000 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/keycloak/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     3199 2023-08-04 09:28:32.000000 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/keycloak/_keycloak_auth.py
+drwxr-xr-x   0 vgurin    (1000) vgurin    (1000)        0 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/redis/
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       49 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/redis/__init__.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)     5056 2023-08-04 09:14:28.000000 py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/redis/_auth_deco.py
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)       38 2023-08-04 09:28:41.371508 py-ke-utils-fastapi-2.1.0/setup.cfg
+-rw-r--r--   0 vgurin    (1000) vgurin    (1000)      728 2023-08-04 09:24:44.000000 py-ke-utils-fastapi-2.1.0/setup.py
```

### Comparing `py-ke-utils-fastapi-2.0.2/README.md` & `py-ke-utils-fastapi-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-2.0.2/pykeutilsfastapi/_auth_deco.py` & `py-ke-utils-fastapi-2.1.0/pykeutilsfastapi/redis/_auth_deco.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 security = HTTPBearer()
 
 
 class JWTSetup:
     """
     Class for storing redis config data
     """
+
     r = None
     channel = None
     pub = None
     res = None
 
     @staticmethod
     def init(r, channel, pub, res):
@@ -39,15 +40,15 @@
         JWTSetup.channel = channel
         JWTSetup.pub = pub
         JWTSetup.res = res
 
 
 async def jwt_redis_auth(credentials: HTTPAuthorizationCredentials = Depends(security)):
     """
-        Function that is used to validate the token in the case that it requires it
+    Function that is used to validate the token in the case that it requires it
     """
     if not JWTSetup.pub or not JWTSetup.res or not JWTSetup.channel or not JWTSetup.r:
         raise redis.exceptions.ConnectionError
     publish_message = copy.deepcopy(JWTSetup.pub)
     response_message = copy.deepcopy(JWTSetup.res)
     token = credentials.credentials
 
@@ -84,28 +85,23 @@
                     continue
                 diff = deepdiff.DeepDiff(response_message, redis_response)
                 if diff == {}:
                     pubsub.unsubscribe(f"{JWTSetup.channel}.reply")
                     redis_client.close()
                     break
                 values = diff.get("values_changed", {})
-                if all(
-                        change["old_value"] != request_id
-                        for change in values.values()
-                ):
+                if all(change["old_value"] != request_id for change in values.values()):
                     pubsub.unsubscribe(f"{JWTSetup.channel}.reply")
                     redis_client.close()
                     raise HTTPException(status_code=401, detail="Unauthorized")
         except TimeoutError as e:
             logging.error("Haven't received any answer from Redis for 5 seconds.")
             pubsub.unsubscribe(f"{JWTSetup.channel}.reply")
             redis_client.close()
-            raise HTTPException(
-                status_code=504, detail="Gateway Timeout"
-            ) from e
+            raise HTTPException(status_code=504, detail="Gateway Timeout") from e
     except redis.exceptions.ConnectionError as e:
         raise HTTPException(status_code=502, detail="Bad Gateway") from e
 
 
 def _transform_dict(data, new_token: str = "", new_id: str = "") -> dict:
     """
     Function to insert into given dictionary `Token` and `ID` fields.
```

### Comparing `py-ke-utils-fastapi-2.0.2/setup.py` & `py-ke-utils-fastapi-2.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from setuptools import setup, find_packages
 
-VERSION = "2.0.2"
-DESCRIPTION = "Utilities with Redis and FastAPI"
+VERSION = "2.1.0"
+DESCRIPTION = "Utilities for FastAPI"
 
 # Setting up
 setup(
     name="py-ke-utils-fastapi",
     version=VERSION,
     author="KE",
     author_email="",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=[
-        "redis>=4.5.0",
-        "deepdiff>=6.2.1",
-        "PyJWT>=2.0.0"
-    ],
+    install_requires=["redis>=4.5.0", "deepdiff>=6.2.1", "fastapi>=0.90"],
     keywords=["python", "FastAPI", "PyJWT", "decorator", "token"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.11",
         "Operating System :: Unix",
         "Operating System :: MacOS",
```

