# Comparing `tmp/b_cfn_api_v2-4.0.0.tar.gz` & `tmp/b_cfn_api_v2-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_cfn_api_v2-4.0.0.tar", last modified: Mon Sep 12 12:21:53 2022, max compression
+gzip compressed data, was "b_cfn_api_v2-5.0.0.tar", last modified: Fri Aug  4 08:07:29 2023, max compression
```

## Comparing `b_cfn_api_v2-4.0.0.tar` & `b_cfn_api_v2-5.0.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7797 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4961 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.173685 b_cfn_api_v2-4.0.0/b_cfn_api_v2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9771 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2/api.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.173685 b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7797 2022-09-12 12:21:53.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-09-12 12:21:53.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-12 12:21:53.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-09-12 12:21:53.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-09-12 12:21:53.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.173685 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1728 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/fixtures/access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/fixtures/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infra_create.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infra_destroy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_api_key_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2078 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_user_pool_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/main_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/user_pool_stack.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_allow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_deny.py
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_allow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_deny.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-12 12:21:53.177685 b_cfn_api_v2-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2858 2022-09-12 12:13:30.000000 b_cfn_api_v2-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/b_cfn_api_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-08-04 08:07:28.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-08-04 08:07:28.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:07:28.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 08:07:28.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 08:07:28.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:28.998121 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/fixtures/access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/fixtures/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infra_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infra_destroy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/api_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_api_key_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_user_pool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/main_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/user_pool_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_allow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_allow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_deny.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:07:29.002121 b_cfn_api_v2-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-08-04 08:00:23.000000 b_cfn_api_v2-5.0.0/setup.py
```

### Comparing `b_cfn_api_v2-4.0.0/HISTORY.md` & `b_cfn_api_v2-5.0.0/HISTORY.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release history
 
+### 5.0.0
+* Upgrade CDK support from v1 to v2.
+* Upgrade GitHub pipelines checkout version from v2 to v3.
+* Set GitHub pipelines node version 18.
+* Set GitHub pipelines python version 3.10.
+
 ### 4.0.0
 * Fix origin paths between pure api or its cloudfront distribution.
   Both should require stage name to be entered as a part of a URL.
   This is a breaking change.
 
 ### 3.1.0
 * Enable easy stage logging.
```

### Comparing `b_cfn_api_v2-4.0.0/LICENSE` & `b_cfn_api_v2-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b_cfn_api_v2-4.0.0/PKG-INFO` & `b_cfn_api_v2-5.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,226 +1,232 @@
 Metadata-Version: 2.1
 Name: b_cfn_api_v2
-Version: 4.0.0
+Version: 5.0.0
 Summary: Convenient wrapper around CfnApi.
 Home-page: https://github.com/biomapas/B.CfnApiV2.git
 License: Apache License 2.0
-Description: # B.CfnApiV2
-        
-        ![Pipeline](https://github.com/Biomapas/B.CfnApiV2/workflows/Pipeline/badge.svg?branch=master)
-        
-        An API Gateway resource that adds convenient functionality over traditional `CfnApi` resource. 
-        It lets you easily enable authorization, stages, and CDNs. 
-        
-        ### Description
-        
-        Essentially this resource is a wrapper resource for `aws_apigatewayv2` module's `CfnApi`. Meaning, 
-        that you can easily swap `CfnApi` and this `Api` resource with no major impact. But why would you 
-        want to switch a traditional `CfnApi` to this one. Mainly these convenient features:
-        - Easy to add `CloudFront` distribution on top of the API (enabling CDN).
-        - Easy to enable `Stage` and attached to the api.
-        - Easy to add authorization with `UserPoolAuthorizer` & `ApiKeyAuthorizer`.
-        
-        ### Remarks
-        
-        [Biomapas](https://www.biomapas.com/) aims to modernise life-science industry by sharing its IT knowledge with other companies and the community. 
-        This is an open source library intended to be used by anyone. 
-        Improvements and pull requests are welcome. 
-        
-        ### Related technology
-        
-        - Python3
-        - AWS CDK
-        - AWS Lambda
-        - AWS API Gateway
-        - AWS CloudFront
-        - AWS User Pool authorization
-        
-        ### Assumptions
-        
-        This project assumes you know what Lambda functions are and how code is being shared between them
-        (Lambda layers). 
-        
-        - Excellent knowledge in IaaC (Infrastructure as a Code) principles.
-        - Excellent knowledge in Lambda functions and API Gateway service.  
-        - Good experience in AWS CDK and AWS CloudFormation.
-        
-        ### Useful sources
-        
-        - AWS CDK:<br>https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html
-        - AWS CloudFormation:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html
-        - AWS API Gateway:<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html
-        - AWS API Gateway V2:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-api.html
-        - Custom User Pool Authorizer:<br>https://github.com/Biomapas/B.CfnCustomUserPoolAuthorizer
-        - Custom api key authorizer:<br>https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer
-        - Custom user pool authorizer:<br>https://github.com/Biomapas/B.CfnCustomUserPoolAuthorizer
-        
-        ### Install
-        
-        Before installing this library, ensure you have these tools setup:
-        
-        - Python / Pip
-        - AWS CDK
-        
-        To install this project from source run:
-        
-        ```
-        pip install .
-        ```
-        
-        
-        Or you can install it from a PyPi repository:
-        
-        ```
-        pip install b-cfn-api-v2
-        ```
-        
-        
-        ### Usage & Examples
-        
-        The traditional way of creating an API looks something like this:
-        
-        ```python
-        from aws_cdk.aws_apigatewayv2 import CfnApi
-        
-        CfnApi(
-            scope=Stack(),
-            id='Api',
-            name='Api',
-            description='Sample description.',
-            protocol_type='HTTP',
-            cors_configuration=CfnApi.CorsProperty(
-                allow_methods=['GET', 'PUT', 'POST', 'OPTIONS', 'DELETE'],
-                allow_origins=['*'],
-                allow_headers=[
-                    'Content-Type',
-                    'Authorization'
-                ],
-                max_age=300
-            )
-        )
-        ```
-        
-        To create our resource `Api` is exactly the same:<br>
-        (It works since `Api` is a pure wrapper of `CfnApi` resource.)
-        
-        ```python
-        from b_cfn_api_v2.api import Api
-        
-        Api(
-            scope=Stack(),
-            id='Api',
-            name='Api',
-            description='Sample description.',
-            protocol_type='HTTP',
-            cors_configuration=Api.CorsProperty(
-                allow_methods=['GET', 'PUT', 'POST', 'OPTIONS', 'DELETE'],
-                allow_origins=['*'],
-                allow_headers=[
-                    'Content-Type',
-                    'Authorization'
-                ],
-                max_age=300
-            )
-        )
-        ```
-        
-        Three main advantages of this `Api` resource:
-        
-        - **Easy to enable default stage.**
-        
-        ```python
-        from b_cfn_api_v2.api import Api
-        
-        api = Api(...)
-        api.enable_default_stage('dev')
-        ```
-        
-        - **Easy to enable authorization.**
-        
-        ```python
-        from b_cfn_api_v2.api import Api
-        from b_cfn_custom_userpool_authorizer.config.user_pool_config import UserPoolConfig
-        
-        api = Api(...)
-        
-        # Your authorized endpoint will require `Authorization`
-        # supplied in headers.
-        # Read more:
-        # https://github.com/Biomapas/B.CfnCustomUserPoolAuthorizer
-        api.enable_user_pool_authorizer(UserPoolConfig(
-            user_pool_id='id',
-            user_pool_region='region',
-            user_pool_client_id='client'
-        ))
-        
-        # Your authorized endpoint will require `ApiKey` and `ApiSecret`
-        # supplied in headers.
-        # Read more:
-        # https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer
-        api.enable_api_key_authorizer()
-        ```
-        
-        - **Easy to enable CDN.**
-        
-        ```python
-        from b_cfn_api_v2.api import Api
-        from aws_cdk.aws_cloudfront import CachePolicy
-        
-        api = Api(...)
-        api.enable_cdn(default_behavior_cache_policy=CachePolicy.CACHING_OPTIMIZED)
-        ```
-        
-        ### Testing
-        
-        This package has integration tests based on **pytest**.
-        To run tests simply run:
-        
-        ```
-        pytest b_cfn_api_v2_test/integration/tests
-        ```
-        
-        ### Contribution
-        
-        Found a bug? Want to add or suggest a new feature? 
-        Contributions of any kind are gladly welcome. 
-        You may contact us directly, create a pull-request or an issue in github platform. 
-        Lets modernize the world together.
-        
-        
-        # Release history
-        
-        ### 4.0.0
-        * Fix origin paths between pure api or its cloudfront distribution.
-          Both should require stage name to be entered as a part of a URL.
-          This is a breaking change.
-        
-        ### 3.1.0
-        * Enable easy stage logging.
-        
-        ### 3.0.0
-        * Upgrade breaking dependencies.
-        
-        ### 2.0.1
-        * Make dependencies range more loose with maximum version not reaching `2.0.0`.
-        
-        ### 2.0.0
-        * Use the newest `2.0.0` custom api keys authorizer which now hashes 
-        api secrets and is no longer compatible with previous versions. 
-        
-        ### 1.1.1
-        * Update readme.
-        
-        ### 1.1.0
-        * Implement api keys custom authorizer (https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer).
-        
-        ### 1.0.0
-        * Fully documented, tested, and working version release.
-        
-        ### 0.0.1
-        * Initial build. 
-        
 Keywords: AWS API Gateway
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# B.CfnApiV2
+
+![Pipeline](https://github.com/Biomapas/B.CfnApiV2/workflows/Pipeline/badge.svg?branch=master)
+
+An API Gateway resource that adds convenient functionality over traditional `CfnApi` resource. 
+It lets you easily enable authorization, stages, and CDNs. 
+
+### Description
+
+Essentially this resource is a wrapper resource for `aws_apigatewayv2` module's `CfnApi`. Meaning, 
+that you can easily swap `CfnApi` and this `Api` resource with no major impact. But why would you 
+want to switch a traditional `CfnApi` to this one. Mainly these convenient features:
+- Easy to add `CloudFront` distribution on top of the API (enabling CDN).
+- Easy to enable `Stage` and attached to the api.
+- Easy to add authorization with `UserPoolAuthorizer` & `ApiKeyAuthorizer`.
+
+### Remarks
+
+[Biomapas](https://www.biomapas.com/) aims to modernise life-science industry by sharing its IT knowledge with other companies and the community. 
+This is an open source library intended to be used by anyone. 
+Improvements and pull requests are welcome. 
+
+### Related technology
+
+- Python3
+- AWS CDK
+- AWS Lambda
+- AWS API Gateway
+- AWS CloudFront
+- AWS User Pool authorization
+
+### Assumptions
+
+This project assumes you know what Lambda functions are and how code is being shared between them
+(Lambda layers). 
+
+- Excellent knowledge in IaaC (Infrastructure as a Code) principles.
+- Excellent knowledge in Lambda functions and API Gateway service.  
+- Good experience in AWS CDK and AWS CloudFormation.
+
+### Useful sources
+
+- AWS CDK:<br>https://docs.aws.amazon.com/cdk/api/latest/docs/aws-construct-library.html
+- AWS CloudFormation:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html
+- AWS API Gateway:<br>https://docs.aws.amazon.com/apigateway/latest/developerguide/welcome.html
+- AWS API Gateway V2:<br>https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-apigatewayv2-api.html
+- Custom User Pool Authorizer:<br>https://github.com/Biomapas/B.CfnCustomUserPoolAuthorizer
+- Custom api key authorizer:<br>https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer
+- Custom user pool authorizer:<br>https://github.com/Biomapas/B.CfnCustomUserPoolAuthorizer
+
+### Install
+
+Before installing this library, ensure you have these tools setup:
+
+- Python / Pip
+- AWS CDK
+
+To install this project from source run:
+
+```
+pip install .
+```
+
+
+Or you can install it from a PyPi repository:
+
+```
+pip install b-cfn-api-v2
+```
+
+
+### Usage & Examples
+
+The traditional way of creating an API looks something like this:
+
+```python
+from aws_cdk.aws_apigatewayv2 import CfnApi
+
+CfnApi(
+    scope=Stack(),
+    id='Api',
+    name='Api',
+    description='Sample description.',
+    protocol_type='HTTP',
+    cors_configuration=CfnApi.CorsProperty(
+        allow_methods=['GET', 'PUT', 'POST', 'OPTIONS', 'DELETE'],
+        allow_origins=['*'],
+        allow_headers=[
+            'Content-Type',
+            'Authorization'
+        ],
+        max_age=300
+    )
+)
+```
+
+To create our resource `Api` is exactly the same:<br>
+(It works since `Api` is a pure wrapper of `CfnApi` resource.)
+
+```python
+from b_cfn_api_v2.api import Api
+
+Api(
+    scope=Stack(),
+    id='Api',
+    name='Api',
+    description='Sample description.',
+    protocol_type='HTTP',
+    cors_configuration=Api.CorsProperty(
+        allow_methods=['GET', 'PUT', 'POST', 'OPTIONS', 'DELETE'],
+        allow_origins=['*'],
+        allow_headers=[
+            'Content-Type',
+            'Authorization'
+        ],
+        max_age=300
+    )
+)
+```
+
+Three main advantages of this `Api` resource:
+
+- **Easy to enable default stage.**
+
+```python
+from b_cfn_api_v2.api import Api
+
+api = Api(...)
+api.enable_default_stage('dev')
+```
+
+- **Easy to enable authorization.**
+
+```python
+from b_cfn_api_v2.api import Api
+from b_cfn_custom_userpool_authorizer.config.user_pool_config import UserPoolConfig
+
+api = Api(...)
+
+# Your authorized endpoint will require `Authorization`
+# supplied in headers.
+# Read more:
+# https://github.com/Biomapas/B.CfnCustomUserPoolAuthorizer
+api.enable_user_pool_authorizer(UserPoolConfig(
+    user_pool_id='id',
+    user_pool_region='region',
+    user_pool_client_id='client'
+))
+
+# Your authorized endpoint will require `ApiKey` and `ApiSecret`
+# supplied in headers.
+# Read more:
+# https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer
+api.enable_api_key_authorizer()
+```
+
+- **Easy to enable CDN.**
+
+```python
+from b_cfn_api_v2.api import Api
+from aws_cdk.aws_cloudfront import CachePolicy
+
+api = Api(...)
+api.enable_cdn(default_behavior_cache_policy=CachePolicy.CACHING_OPTIMIZED)
+```
+
+### Testing
+
+This package has integration tests based on **pytest**.
+To run tests simply run:
+
+```
+pytest b_cfn_api_v2_test/integration/tests
+```
+
+### Contribution
+
+Found a bug? Want to add or suggest a new feature? 
+Contributions of any kind are gladly welcome. 
+You may contact us directly, create a pull-request or an issue in github platform. 
+Lets modernize the world together.
+
+
+# Release history
+
+### 5.0.0
+* Upgrade CDK support from v1 to v2.
+* Upgrade GitHub pipelines checkout version from v2 to v3.
+* Set GitHub pipelines node version 18.
+* Set GitHub pipelines python version 3.10.
+
+### 4.0.0
+* Fix origin paths between pure api or its cloudfront distribution.
+  Both should require stage name to be entered as a part of a URL.
+  This is a breaking change.
+
+### 3.1.0
+* Enable easy stage logging.
+
+### 3.0.0
+* Upgrade breaking dependencies.
+
+### 2.0.1
+* Make dependencies range more loose with maximum version not reaching `2.0.0`.
+
+### 2.0.0
+* Use the newest `2.0.0` custom api keys authorizer which now hashes 
+api secrets and is no longer compatible with previous versions. 
+
+### 1.1.1
+* Update readme.
+
+### 1.1.0
+* Implement api keys custom authorizer (https://github.com/Biomapas/B.CfnCustomApiKeyAuthorizer).
+
+### 1.0.0
+* Fully documented, tested, and working version release.
+
+### 0.0.1
+* Initial build.
```

### Comparing `b_cfn_api_v2-4.0.0/README.md` & `b_cfn_api_v2-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2/api.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import json
 from typing import Optional, Any, Union, Dict
 
+from aws_cdk import Stack, IResolvable, RemovalPolicy
 from aws_cdk.aws_apigatewayv2 import CfnApi, CfnStage
 from aws_cdk.aws_cloudfront import *
 from aws_cdk.aws_cloudfront_origins import HttpOrigin
 from aws_cdk.aws_iam import ServicePrincipal
 from aws_cdk.aws_logs import LogGroup, RetentionDays
 from aws_cdk.aws_ssm import StringParameter
-from aws_cdk.core import Stack, IResolvable, RemovalPolicy
 from b_cfn_custom_api_key_authorizer.custom_authorizer import ApiKeyCustomAuthorizer
 from b_cfn_custom_userpool_authorizer.config.user_pool_config import UserPoolConfig
 from b_cfn_custom_userpool_authorizer.config.user_pool_ssm_config import UserPoolSsmConfig
 from b_cfn_custom_userpool_authorizer.user_pool_custom_authorizer import UserPoolCustomAuthorizer
 
 
 class Api(CfnApi):
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2.egg-info/SOURCES.txt` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 b_cfn_api_v2_test/integration/infra_create.py
 b_cfn_api_v2_test/integration/infra_destroy.py
 b_cfn_api_v2_test/integration/manager.py
 b_cfn_api_v2_test/integration/fixtures/__init__.py
 b_cfn_api_v2_test/integration/fixtures/access_token.py
 b_cfn_api_v2_test/integration/fixtures/api_keys.py
 b_cfn_api_v2_test/integration/infrastructure/__init__.py
+b_cfn_api_v2_test/integration/infrastructure/api_stack.py
 b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_api_key_stack.py
 b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_user_pool_stack.py
 b_cfn_api_v2_test/integration/infrastructure/main_stack.py
 b_cfn_api_v2_test/integration/infrastructure/user_pool_stack.py
 b_cfn_api_v2_test/integration/tests/__init__.py
 b_cfn_api_v2_test/integration/tests/test_api_api_key_allow.py
 b_cfn_api_v2_test/integration/tests/test_api_api_key_deny.py
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/fixtures/access_token.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/fixtures/access_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from b_aws_testing_framework.credentials import Credentials
-from b_cfn_api_v2_test.integration.infrastructure.main_stack import MainStack
 from pytest import fixture
 
+from b_cfn_api_v2_test.integration.infrastructure.main_stack import MainStack
+
 
 @fixture(scope='function')
 def access_token():
     client = Credentials().boto_session.client('cognito-idp')
     user_pool_id = MainStack.get_output(MainStack.USER_POOL_ID_KEY)
     user_pool_client_id = MainStack.get_output(MainStack.USER_POOL_CLIENT_ID_KEY)
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/fixtures/api_keys.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/fixtures/api_keys.py`

 * *Files identical despite different names*

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_api_key_stack.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_user_pool_stack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_apigatewayv2 import CfnRoute
 from aws_cdk.aws_lambda import Function, Code, Runtime, CfnPermission
-from aws_cdk.core import Stack, Duration
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 from b_cfn_lambda_integration.lambda_integration import LambdaIntegration
 
 from b_cfn_api_v2.api import Api
 
 
-class AuthorizedEndpointApiKeyStack(Stack):
+class AuthorizedEndpointUserPoolStack(Stack):
     def __init__(self, scope: Stack, api: Api):
         super().__init__(
             scope=scope,
-            id='ApiKeyAuthorizedEndpointStack'
+            id='UserPoolAuthorizedEndpointStack'
         )
 
         prefix = TestingStack.global_prefix()
 
         self.api_endpoint_function = Function(
             scope=self,
-            id='ApiFunction2',
-            function_name=f'{prefix}ApiFunction2',
+            id='ApiFunction1',
+            function_name=f'{prefix}ApiFunction1',
             code=Code.from_inline(
                 'def handler(event, context):\n'
                 '    print(event)\n'
                 '    return {\n'
                 '        "statusCode": 200,\n'
                 '        "headers": {},\n'
                 '        "body": "Hello World!",\n'
@@ -43,20 +43,20 @@
             function_name=self.api_endpoint_function.function_name,
             principal='apigateway.amazonaws.com',
         )
 
         self.integration = LambdaIntegration(
             scope=self,
             api=api,
-            integration_name=f'{prefix}Integration2',
+            integration_name=f'{prefix}Integration1',
             lambda_function=self.api_endpoint_function
         )
 
         self.route = CfnRoute(
             scope=self,
             id='DummyRoute',
             api_id=api.ref,
-            route_key=f'GET /dummy2',
+            route_key=f'GET /dummy1',
             authorization_type='CUSTOM',
             target=f'integrations/{self.integration.ref}',
-            authorizer_id=api.api_key_authorizer.ref
+            authorizer_id=api.authorizer.ref
         )
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_user_pool_stack.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/authorized_endpoint_api_key_stack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+from aws_cdk import Stack, Duration
 from aws_cdk.aws_apigatewayv2 import CfnRoute
 from aws_cdk.aws_lambda import Function, Code, Runtime, CfnPermission
-from aws_cdk.core import Stack, Duration
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 from b_cfn_lambda_integration.lambda_integration import LambdaIntegration
 
 from b_cfn_api_v2.api import Api
 
 
-class AuthorizedEndpointUserPoolStack(Stack):
+class AuthorizedEndpointApiKeyStack(Stack):
     def __init__(self, scope: Stack, api: Api):
         super().__init__(
             scope=scope,
-            id='UserPoolAuthorizedEndpointStack'
+            id='ApiKeyAuthorizedEndpointStack'
         )
 
         prefix = TestingStack.global_prefix()
 
         self.api_endpoint_function = Function(
             scope=self,
-            id='ApiFunction1',
-            function_name=f'{prefix}ApiFunction1',
+            id='ApiFunction2',
+            function_name=f'{prefix}ApiFunction2',
             code=Code.from_inline(
                 'def handler(event, context):\n'
                 '    print(event)\n'
                 '    return {\n'
                 '        "statusCode": 200,\n'
                 '        "headers": {},\n'
                 '        "body": "Hello World!",\n'
@@ -43,20 +43,20 @@
             function_name=self.api_endpoint_function.function_name,
             principal='apigateway.amazonaws.com',
         )
 
         self.integration = LambdaIntegration(
             scope=self,
             api=api,
-            integration_name=f'{prefix}Integration1',
+            integration_name=f'{prefix}Integration2',
             lambda_function=self.api_endpoint_function
         )
 
         self.route = CfnRoute(
             scope=self,
             id='DummyRoute',
             api_id=api.ref,
-            route_key=f'GET /dummy1',
+            route_key=f'GET /dummy2',
             authorization_type='CUSTOM',
             target=f'integrations/{self.integration.ref}',
-            authorizer_id=api.authorizer.ref
+            authorizer_id=api.api_key_authorizer.ref
         )
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/infrastructure/user_pool_stack.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/infrastructure/user_pool_stack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from aws_cdk.aws_cognito import *
+from aws_cdk import Stack
+from aws_cdk.aws_cognito import UserPool, AccountRecovery, AutoVerifiedAttrs, SignInAliases, StandardAttributes, StandardAttribute, UserPoolClient, AuthFlow
 from aws_cdk.aws_ssm import StringParameter
-from aws_cdk.core import Stack
 from b_aws_testing_framework.tools.cdk_testing.testing_stack import TestingStack
 
 
 class UserPoolStack(Stack):
     def __init__(self, scope: Stack):
         super().__init__(
             scope=scope,
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/manager.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,8 +5,8 @@
 from b_aws_testing_framework.tools.cdk_testing.testing_manager import TestingManager
 
 GLOBAL_PREFIX = os.environ.get('GLOBAL_PREFIX')
 CDK_PATH = f'{os.path.dirname(os.path.abspath(__file__))}'
 MANAGER = TestingManager(Credentials(), CdkToolConfig(CDK_PATH, destroy_before_preparing=False))
 
 if GLOBAL_PREFIX:
-    MANAGER.set_global_prefix(f'B{GLOBAL_PREFIX[:10]}')
+    MANAGER.set_global_prefix(GLOBAL_PREFIX[:10])
```

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_allow.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_allow.py`

 * *Files identical despite different names*

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_deny.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_api_key_deny.py`

 * *Files identical despite different names*

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_allow.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_allow.py`

 * *Files identical despite different names*

### Comparing `b_cfn_api_v2-4.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_deny.py` & `b_cfn_api_v2-5.0.0/b_cfn_api_v2_test/integration/tests/test_api_user_pool_deny.py`

 * *Files identical despite different names*

