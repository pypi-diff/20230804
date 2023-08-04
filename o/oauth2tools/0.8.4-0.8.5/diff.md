# Comparing `tmp/oauth2tools-0.8.4.tar.gz` & `tmp/oauth2tools-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2tools-0.8.4.tar", last modified: Sun Nov 27 14:29:13 2022, max compression
+gzip compressed data, was "oauth2tools-0.8.5.tar", last modified: Fri Aug  4 15:38:33 2023, max compression
```

## Comparing `oauth2tools-0.8.4.tar` & `oauth2tools-0.8.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 14:29:13.604155 oauth2tools-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-11-27 14:29:13.604155 oauth2tools-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 14:29:13.604155 oauth2tools-0.8.4/oauth2tools/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/jwt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/oauth2tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/oauth4cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 14:29:13.604155 oauth2tools-0.8.4/oauth2tools/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/templates/close_me.html
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/oauth2tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-27 14:29:13.604155 oauth2tools-0.8.4/oauth2tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2022-11-27 14:29:13.000000 oauth2tools-0.8.4/oauth2tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2022-11-27 14:29:13.000000 oauth2tools-0.8.4/oauth2tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-27 14:29:13.000000 oauth2tools-0.8.4/oauth2tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-11-27 14:29:13.000000 oauth2tools-0.8.4/oauth2tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-11-27 14:29:13.000000 oauth2tools-0.8.4/oauth2tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      819 2022-11-27 14:29:03.000000 oauth2tools-0.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-11-27 14:29:13.604155 oauth2tools-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:33.265758 oauth2tools-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-04 15:38:33.265758 oauth2tools-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:33.265758 oauth2tools-0.8.5/oauth2tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/jwt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/oauth2tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/oauth4cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:33.265758 oauth2tools-0.8.5/oauth2tools/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/templates/close_me.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/oauth2tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:38:33.265758 oauth2tools-0.8.5/oauth2tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-08-04 15:38:33.000000 oauth2tools-0.8.5/oauth2tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-08-04 15:38:33.000000 oauth2tools-0.8.5/oauth2tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:38:33.000000 oauth2tools-0.8.5/oauth2tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 15:38:33.000000 oauth2tools-0.8.5/oauth2tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 15:38:33.000000 oauth2tools-0.8.5/oauth2tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 15:38:21.000000 oauth2tools-0.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:38:33.265758 oauth2tools-0.8.5/setup.cfg
```

### Comparing `oauth2tools-0.8.4/LICENSE` & `oauth2tools-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2tools-0.8.4/PKG-INFO` & `oauth2tools-0.8.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2tools
-Version: 0.8.4
+Version: 0.8.5
 Summary: A toolset for the most requirements dealing with OAuth2 and OpenID Connect.
 Author: Andreas Rühl
 Maintainer: Andreas Rühl
 License: MIT
 Project-URL: GitHub, https://github.com/aruehl/oauth2tools
 Project-URL: Bug Tracker, https://github.com/aruehl/oauth2tools/issues
 Keywords: OAuth2,OIDC,OpenID Connect,Tools,Helper
```

### Comparing `oauth2tools-0.8.4/README.md` & `oauth2tools-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `oauth2tools-0.8.4/oauth2tools/jwt_helper.py` & `oauth2tools-0.8.5/oauth2tools/jwt_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     else:
         return claim_value
 
 
 def validate_by_key(token: str, signing_key: str, algorithms: list = None, **kwargs) -> dict:
     """
     Using PyJWT (https://pyjwt.readthedocs.io/en/latest/usage.html) to validate the JWT.
-    Algorithms are restricted to RS256 and ES256 by default.
+    Algorithms are restricted to RS256, RS384, RS512, ES256, ES384 and ES512 by default.
     All keyword arguments are bypassed. For example:
     issuer="https://www.example.com/idp/test"
     audience=["my_service"]
     options={"verify_aud": False}
     Additional claims to be checked can be passed within the claims param. For example:
     The 'groups' claim must be equal to or contain the 'my_group'
     claims={"groups": "my_group"}
@@ -53,15 +53,15 @@
     :param token: the jwt
     :param signing_key: the public key for checking the signature
     :param algorithms: list of valid algorithms
     :param kwargs: everything supported by the PyJWT module
     :return: decoded body
     """
     if algorithms is None:
-        algorithms = ["ES256", "RS256"]
+        algorithms = ["ES256", "ES384", "ES512", "RS256", "RS384", "RS512"]
     if "leeway" not in kwargs:
         kwargs["leeway"] = 5
     decoded = jwt.decode(
         token,
         signing_key,
         algorithms=algorithms,
         **kwargs
```

### Comparing `oauth2tools-0.8.4/oauth2tools/oauth2tools.py` & `oauth2tools-0.8.5/oauth2tools/oauth2tools.py`

 * *Files identical despite different names*

### Comparing `oauth2tools-0.8.4/oauth2tools/oauth4cli.py` & `oauth2tools-0.8.5/oauth2tools/oauth4cli.py`

 * *Files identical despite different names*

### Comparing `oauth2tools-0.8.4/oauth2tools/templates/close_me.html` & `oauth2tools-0.8.5/oauth2tools/templates/close_me.html`

 * *Files identical despite different names*

### Comparing `oauth2tools-0.8.4/oauth2tools/tools.py` & `oauth2tools-0.8.5/oauth2tools/tools.py`

 * *Files identical despite different names*

### Comparing `oauth2tools-0.8.4/oauth2tools.egg-info/PKG-INFO` & `oauth2tools-0.8.5/oauth2tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2tools
-Version: 0.8.4
+Version: 0.8.5
 Summary: A toolset for the most requirements dealing with OAuth2 and OpenID Connect.
 Author: Andreas Rühl
 Maintainer: Andreas Rühl
 License: MIT
 Project-URL: GitHub, https://github.com/aruehl/oauth2tools
 Project-URL: Bug Tracker, https://github.com/aruehl/oauth2tools/issues
 Keywords: OAuth2,OIDC,OpenID Connect,Tools,Helper
```

### Comparing `oauth2tools-0.8.4/pyproject.toml` & `oauth2tools-0.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oauth2tools"
-version = "0.8.4"
+version = "0.8.5"
 description = "A toolset for the most requirements dealing with OAuth2 and OpenID Connect."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 keywords = [ "OAuth2", "OIDC", "OpenID Connect", "Tools", "Helper",]
 dependencies = [ "flask", "requests", "werkzeug",]
 [[project.authors]]
```

