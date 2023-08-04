# Comparing `tmp/usermgr-0.1.2.tar.gz` & `tmp/usermgr-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usermgr-0.1.2.tar", max compression
+gzip compressed data, was "usermgr-0.2.0.tar", max compression
```

## Comparing `usermgr-0.1.2.tar` & `usermgr-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.1.2/LICENSE
--rw-r--r--   0        0        0      411 2023-07-31 06:02:25.989115 usermgr-0.1.2/README.md
--rw-r--r--   0        0        0      588 2023-07-31 05:59:49.069134 usermgr-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      313 2023-06-24 05:20:14.654589 usermgr-0.1.2/usermgr/Factory.py
--rw-r--r--   0        0        0       22 2023-07-31 05:59:40.199134 usermgr-0.1.2/usermgr/__init__.py
--rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.1.2/usermgr/base.py
--rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.1.2/usermgr/providers/__init__.py
--rw-r--r--   0        0        0     3656 2023-07-31 05:54:04.809152 usermgr-0.1.2/usermgr/providers/cognito.py
--rw-r--r--   0        0        0      977 1970-01-01 00:00:00.000000 usermgr-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-24 05:20:14.654589 usermgr-0.2.0/LICENSE
+-rw-r--r--   0        0        0      407 2023-07-31 06:05:17.779124 usermgr-0.2.0/README.md
+-rw-r--r--   0        0        0      607 2023-08-04 03:57:13.879824 usermgr-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      335 2023-08-02 17:01:51.661912 usermgr-0.2.0/usermgr/Factory.py
+-rw-r--r--   0        0        0       22 2023-08-04 03:56:14.259827 usermgr-0.2.0/usermgr/__init__.py
+-rw-r--r--   0        0        0      994 2023-06-24 13:09:02.722831 usermgr-0.2.0/usermgr/base.py
+-rw-r--r--   0        0        0        0 2023-06-24 05:20:14.654589 usermgr-0.2.0/usermgr/providers/__init__.py
+-rw-r--r--   0        0        0     3656 2023-07-31 05:54:04.809152 usermgr-0.2.0/usermgr/providers/cognito.py
+-rw-r--r--   0        0        0     2125 2023-08-04 03:49:19.409848 usermgr-0.2.0/usermgr/providers/lambda.py
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 usermgr-0.2.0/PKG-INFO
```

### Comparing `usermgr-0.1.2/LICENSE` & `usermgr-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.2/pyproject.toml` & `usermgr-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "usermgr"
-version = "0.1.2"
+version = "0.2.0"
 description = ""
 authors = ["tamuto <tamuto@infodb.jp>"]
 readme = "README.md"
 homepage = "https://github.com/tamuto/usermgr"
 repository = "https://github.com/tamuto/usermgr"
 
 packages = [
@@ -13,14 +13,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3 = {version = "^1.26.54", optional = true}
 
 [tool.poetry.extras]
 cognito = ["boto3"]
+lambda = ["boto3"]
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = {extras = ["cli"], version = "^0.21.1"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `usermgr-0.1.2/usermgr/base.py` & `usermgr-0.2.0/usermgr/base.py`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.2/usermgr/providers/cognito.py` & `usermgr-0.2.0/usermgr/providers/cognito.py`

 * *Files identical despite different names*

### Comparing `usermgr-0.1.2/PKG-INFO` & `usermgr-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: usermgr
-Version: 0.1.2
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/tamuto/usermgr
 Author: tamuto
 Author-email: tamuto@infodb.jp
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cognito
-Requires-Dist: boto3 (>=1.26.54,<2.0.0) ; extra == "cognito"
+Provides-Extra: lambda
+Requires-Dist: boto3 (>=1.26.54,<2.0.0) ; extra == "cognito" or extra == "lambda"
 Project-URL: Repository, https://github.com/tamuto/usermgr
 Description-Content-Type: text/markdown
 
 # User Management API
 
 ## Memo
 
@@ -25,15 +26,15 @@
 
 ```
 AWS_ACCESS_KEY_ID=***
 AWS_SECRET_ACCESS_KEY=***
 or
 AWS_PROFILE=***
 
-AWS_REGION=***
+REGION=***
 USER_POOL_ID=***
 CLIENT_ID=***
 CLIENT_SECRET=***
 ```
 
   * run unittest
```

