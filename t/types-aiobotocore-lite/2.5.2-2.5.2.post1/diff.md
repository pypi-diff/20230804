# Comparing `tmp/types-aiobotocore-lite-2.5.2.tar.gz` & `tmp/types-aiobotocore-lite-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lite-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-lite-2.5.2.post1.tar", last modified: Fri Aug  4 14:07:59 2023, max compression
```

## Comparing `types-aiobotocore-lite-2.5.2.tar` & `types-aiobotocore-lite-2.5.2.post1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.749697 types-aiobotocore-lite-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:11.000000 types-aiobotocore-lite-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    81849 2023-07-08 01:43:14.745697 types-aiobotocore-lite-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    70395 2023-07-08 01:25:11.000000 types-aiobotocore-lite-2.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.737697 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/args.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/awsrequest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/configprovider.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/eventstream.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/httpchecksum.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/httpsession.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/paginate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/parsers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:11.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/retryhandler.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/signers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:11.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-08 01:25:10.000000 types-aiobotocore-lite-2.5.2/aiobotocore-stubs/waiter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.749697 types-aiobotocore-lite-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    49563 2023-07-08 01:25:11.000000 types-aiobotocore-lite-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.745697 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    81849 2023-07-08 01:43:14.000000 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-08 01:43:14.000000 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    36717 2023-07-08 01:43:14.000000 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-08 01:43:14.000000 types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:59.496649 types-aiobotocore-lite-2.5.2.post1/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 14:07:31.000000 types-aiobotocore-lite-2.5.2.post1/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    82708 2023-08-04 14:07:59.496649 types-aiobotocore-lite-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    71117 2023-08-04 14:07:31.000000 types-aiobotocore-lite-2.5.2.post1/README.md
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:59.496649 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       17 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1627 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/args.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      175 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/awsrequest.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1357 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      300 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/config.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      399 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/configprovider.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5731 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/credentials.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/discovery.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1467 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/endpoint.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      394 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/eventstream.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      595 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/handlers.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      261 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/hooks.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      643 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/httpchecksum.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      968 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/httpsession.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      732 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/paginate.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      745 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/parsers.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:31.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      541 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/regions.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1389 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/response.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/retryhandler.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2695 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/session.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2182 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/signers.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/tokens.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2147 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/utils.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      581 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/waiter.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 14:07:59.496649 types-aiobotocore-lite-2.5.2.post1/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    50157 2023-08-04 14:07:30.000000 types-aiobotocore-lite-2.5.2.post1/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 14:07:59.496649 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    82708 2023-08-04 14:07:59.000000 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1075 2023-08-04 14:07:59.000000 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 14:07:59.000000 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 14:07:59.000000 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37185 2023-08-04 14:07:59.000000 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       18 2023-08-04 14:07:59.000000 types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lite-2.5.2/LICENSE` & `types-aiobotocore-lite-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/PKG-INFO` & `types-aiobotocore-lite-2.5.2.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lite
-Version: 2.5.2
-Summary: Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -41,14 +41,15 @@
 Provides-Extra: amplifybackend
 Provides-Extra: amplifyuibuilder
 Provides-Extra: apigateway
 Provides-Extra: apigatewaymanagementapi
 Provides-Extra: apigatewayv2
 Provides-Extra: appconfig
 Provides-Extra: appconfigdata
+Provides-Extra: appfabric
 Provides-Extra: appflow
 Provides-Extra: appintegrations
 Provides-Extra: application-autoscaling
 Provides-Extra: application-insights
 Provides-Extra: applicationcostprofiler
 Provides-Extra: appmesh
 Provides-Extra: apprunner
@@ -144,14 +145,15 @@
 Provides-Extra: elasticbeanstalk
 Provides-Extra: elastictranscoder
 Provides-Extra: elb
 Provides-Extra: elbv2
 Provides-Extra: emr
 Provides-Extra: emr-containers
 Provides-Extra: emr-serverless
+Provides-Extra: entityresolution
 Provides-Extra: es
 Provides-Extra: events
 Provides-Extra: evidently
 Provides-Extra: finspace
 Provides-Extra: finspace-data
 Provides-Extra: firehose
 Provides-Extra: fis
@@ -230,26 +232,28 @@
 Provides-Extra: lookoutmetrics
 Provides-Extra: lookoutvision
 Provides-Extra: m2
 Provides-Extra: machinelearning
 Provides-Extra: macie
 Provides-Extra: macie2
 Provides-Extra: managedblockchain
+Provides-Extra: managedblockchain-query
 Provides-Extra: marketplace-catalog
 Provides-Extra: marketplace-entitlement
 Provides-Extra: marketplacecommerceanalytics
 Provides-Extra: mediaconnect
 Provides-Extra: mediaconvert
 Provides-Extra: medialive
 Provides-Extra: mediapackage
 Provides-Extra: mediapackage-vod
 Provides-Extra: mediapackagev2
 Provides-Extra: mediastore
 Provides-Extra: mediastore-data
 Provides-Extra: mediatailor
+Provides-Extra: medical-imaging
 Provides-Extra: memorydb
 Provides-Extra: meteringmarketplace
 Provides-Extra: mgh
 Provides-Extra: mgn
 Provides-Extra: migration-hub-refactor-spaces
 Provides-Extra: migrationhub-config
 Provides-Extra: migrationhuborchestrator
@@ -385,29 +389,29 @@
 <a id="types-aiobotocore-lite"></a>
 
 # types-aiobotocore-lite
 
 [![PyPI - types-aiobotocore-lite](https://img.shields.io/pypi/v/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lite.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lite?color=blue)](https://pypistats.org/packages/types-aiobotocore-lite)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lite)](https://pepy.tech/project/types-aiobotocore-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore 2.5.2](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aiobotocore-lite docs](https://youtype.github.io/types_aiobotocore_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -678,15 +682,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `types-aiobotocore-lite[all]` - Type annotations for all 349 services.
+- `types-aiobotocore-lite[all]` - Type annotations for all 353 services.
 - `types-aiobotocore-lite[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/),
   [DynamoDB](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/),
   [EC2](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/),
   [Lambda](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/),
   [RDS](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/),
   [S3](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
@@ -733,14 +737,17 @@
   service.
 - `types-aiobotocore-lite[appconfig]` - Type annotations for
   [AppConfig](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
   service.
 - `types-aiobotocore-lite[appconfigdata]` - Type annotations for
   [AppConfigData](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
   service.
+- `types-aiobotocore-lite[appfabric]` - Type annotations for
+  [AppFabric](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/)
+  service.
 - `types-aiobotocore-lite[appflow]` - Type annotations for
   [Appflow](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
   service.
 - `types-aiobotocore-lite[appintegrations]` - Type annotations for
   [AppIntegrationsService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
   service.
 - `types-aiobotocore-lite[application-autoscaling]` - Type annotations for
@@ -1042,14 +1049,17 @@
   service.
 - `types-aiobotocore-lite[emr-containers]` - Type annotations for
   [EMRContainers](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
   service.
 - `types-aiobotocore-lite[emr-serverless]` - Type annotations for
   [EMRServerless](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
   service.
+- `types-aiobotocore-lite[entityresolution]` - Type annotations for
+  [EntityResolution](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
+  service.
 - `types-aiobotocore-lite[es]` - Type annotations for
   [ElasticsearchService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
   service.
 - `types-aiobotocore-lite[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
   service.
 - `types-aiobotocore-lite[evidently]` - Type annotations for
@@ -1302,14 +1312,17 @@
   service.
 - `types-aiobotocore-lite[macie2]` - Type annotations for
   [Macie2](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
   service.
 - `types-aiobotocore-lite[managedblockchain]` - Type annotations for
   [ManagedBlockchain](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
   service.
+- `types-aiobotocore-lite[managedblockchain-query]` - Type annotations for
+  [ManagedBlockchainQuery](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/)
+  service.
 - `types-aiobotocore-lite[marketplace-catalog]` - Type annotations for
   [MarketplaceCatalog](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
   service.
 - `types-aiobotocore-lite[marketplace-entitlement]` - Type annotations for
   [MarketplaceEntitlementService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
   service.
 - `types-aiobotocore-lite[marketplacecommerceanalytics]` - Type annotations for
@@ -1338,14 +1351,17 @@
   service.
 - `types-aiobotocore-lite[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
   service.
 - `types-aiobotocore-lite[mediatailor]` - Type annotations for
   [MediaTailor](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/)
   service.
+- `types-aiobotocore-lite[medical-imaging]` - Type annotations for
+  [HealthImaging](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
+  service.
 - `types-aiobotocore-lite[memorydb]` - Type annotations for
   [MemoryDB](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/)
   service.
 - `types-aiobotocore-lite[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/)
   service.
 - `types-aiobotocore-lite[mgh]` - Type annotations for
```

### Comparing `types-aiobotocore-lite-2.5.2/README.md` & `types-aiobotocore-lite-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-lite"></a>
 
 # types-aiobotocore-lite
 
 [![PyPI - types-aiobotocore-lite](https://img.shields.io/pypi/v/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lite.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lite?color=blue)](https://pypistats.org/packages/types-aiobotocore-lite)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lite)](https://pepy.tech/project/types-aiobotocore-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore 2.5.2](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aiobotocore-lite docs](https://youtype.github.io/types_aiobotocore_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -294,15 +294,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `types-aiobotocore-lite[all]` - Type annotations for all 349 services.
+- `types-aiobotocore-lite[all]` - Type annotations for all 353 services.
 - `types-aiobotocore-lite[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/),
   [DynamoDB](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/),
   [EC2](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/),
   [Lambda](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/),
   [RDS](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/),
   [S3](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
@@ -349,14 +349,17 @@
   service.
 - `types-aiobotocore-lite[appconfig]` - Type annotations for
   [AppConfig](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
   service.
 - `types-aiobotocore-lite[appconfigdata]` - Type annotations for
   [AppConfigData](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
   service.
+- `types-aiobotocore-lite[appfabric]` - Type annotations for
+  [AppFabric](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/)
+  service.
 - `types-aiobotocore-lite[appflow]` - Type annotations for
   [Appflow](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
   service.
 - `types-aiobotocore-lite[appintegrations]` - Type annotations for
   [AppIntegrationsService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
   service.
 - `types-aiobotocore-lite[application-autoscaling]` - Type annotations for
@@ -658,14 +661,17 @@
   service.
 - `types-aiobotocore-lite[emr-containers]` - Type annotations for
   [EMRContainers](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
   service.
 - `types-aiobotocore-lite[emr-serverless]` - Type annotations for
   [EMRServerless](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
   service.
+- `types-aiobotocore-lite[entityresolution]` - Type annotations for
+  [EntityResolution](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
+  service.
 - `types-aiobotocore-lite[es]` - Type annotations for
   [ElasticsearchService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
   service.
 - `types-aiobotocore-lite[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
   service.
 - `types-aiobotocore-lite[evidently]` - Type annotations for
@@ -918,14 +924,17 @@
   service.
 - `types-aiobotocore-lite[macie2]` - Type annotations for
   [Macie2](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
   service.
 - `types-aiobotocore-lite[managedblockchain]` - Type annotations for
   [ManagedBlockchain](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
   service.
+- `types-aiobotocore-lite[managedblockchain-query]` - Type annotations for
+  [ManagedBlockchainQuery](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/)
+  service.
 - `types-aiobotocore-lite[marketplace-catalog]` - Type annotations for
   [MarketplaceCatalog](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
   service.
 - `types-aiobotocore-lite[marketplace-entitlement]` - Type annotations for
   [MarketplaceEntitlementService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
   service.
 - `types-aiobotocore-lite[marketplacecommerceanalytics]` - Type annotations for
@@ -954,14 +963,17 @@
   service.
 - `types-aiobotocore-lite[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
   service.
 - `types-aiobotocore-lite[mediatailor]` - Type annotations for
   [MediaTailor](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/)
   service.
+- `types-aiobotocore-lite[medical-imaging]` - Type annotations for
+  [HealthImaging](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
+  service.
 - `types-aiobotocore-lite[memorydb]` - Type annotations for
   [MemoryDB](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/)
   service.
 - `types-aiobotocore-lite[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/)
   service.
 - `types-aiobotocore-lite[mgh]` - Type annotations for
```

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/args.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/args.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -38,8 +38,11 @@
         is_secure: bool,
         endpoint_url: str,
         verify: Optional[Union[str, bool]],
         credentials: Credentials,
         scoped_config: Optional[Dict[str, Any]],
         client_config: Optional[Config],
         endpoint_bridge: ClientEndpointBridge,
+        auth_token: Optional[str] = ...,
+        endpoints_ruleset_data: Optional[Dict[str, Any]] = ...,
+        partition_data: Optional[Dict[str, Any]] = ...,
     ) -> _GetClientArgsTypeDef: ...
```

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/client.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         is_secure: bool = ...,
         endpoint_url: Optional[str] = ...,
         verify: Optional[Union[str, bool]] = ...,
         credentials: Optional[Any] = ...,
         scoped_config: Optional[Any] = ...,
         api_version: Optional[str] = ...,
         client_config: Optional[Config] = ...,
+        auth_token: Optional[str] = ...,
     ) -> AioBaseClient: ...
 
 class AioBaseClient(BaseClient):
     def get_paginator(self, operation_name: str) -> AioPaginator: ...
     def get_waiter(self, waiter_name: str) -> AIOWaiter: ...
     async def __aenter__(self: _R) -> _R: ...
     async def __aexit__(
```

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/credentials.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/credentials.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     ProcessProvider,
     ProfileProviderBuilder,
     ReadOnlyCredentials,
     RefreshableCredentials,
     SharedCredentialProvider,
     SSOProvider,
 )
+from botocore.tokens import SSOTokenProvider
+from botocore.utils import SSOTokenLoader
 
 logger: logging.Logger
 
 def create_credential_resolver(
     session: AioSession,
     cache: Optional[Any] = ...,
     region_name: Optional[str] = ...,
@@ -142,14 +144,16 @@
     def __init__(
         self,
         start_url: str,
         sso_region: str,
         role_name: str,
         account_id: str,
         client_creator: Any,
-        token_loader: Optional[Any] = ...,
+        token_loader: Optional[SSOTokenLoader] = ...,
         cache: Optional[Any] = ...,
         expiry_window_seconds: Optional[Any] = ...,
+        token_provider: Optional[SSOTokenProvider] = ...,
+        sso_session_name: Optional[str] = ...,
     ) -> None: ...
 
 class AioSSOProvider(SSOProvider):
     async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore [override]
```

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/endpoint.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/handlers.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/httpchecksum.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/httpsession.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/paginate.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/paginate.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Iterator, Type
+from typing import Any, AsyncIterator, Iterator, Type
 
 from botocore.paginate import PageIterator, Paginator
 
 class AioPageIterator(PageIterator):
     def __aiter__(self) -> Any: ...
     resume_token: Any
-    async def __anext__(self) -> Iterator[Any]: ...
+    async def __anext__(self) -> Any: ...
     def result_key_iters(self) -> Any: ...
     async def build_full_result(self) -> Any: ...
     async def search(self, expression: str) -> Iterator[Any]: ...  # type: ignore [override]
 
 class AioPaginator(Paginator):
     PAGE_ITERATOR_CLS: Type[AioPageIterator]
 
 class ResultKeyIterator:
     result_key: str
     def __init__(self, pages_iterator: PageIterator, result_key: str) -> None: ...
-    def __aiter__(self) -> Any: ...
-    async def __anext__(self) -> Iterator[Any]: ...
+    def __aiter__(self) -> AsyncIterator[Any]: ...
+    async def __anext__(self) -> Any: ...
```

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/parsers.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/response.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/retryhandler.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/session.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/signers.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/signers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/utils.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/utils.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from botocore.utils import (
     ContainerMetadataFetcher,
     IMDSFetcher,
     IMDSRegionProvider,
     InstanceMetadataFetcher,
     InstanceMetadataRegionFetcher,
     S3RegionRedirector,
+    S3RegionRedirectorv2,
 )
 from requests.models import Response
 
 logger: Any
 RETRYABLE_HTTP_ERRORS: Any
 
 class AioIMDSFetcher(IMDSFetcher):
@@ -32,14 +33,24 @@
 
 class AioIMDSRegionProvider(IMDSRegionProvider):
     async def provide(self) -> str: ...
 
 class AioInstanceMetadataRegionFetcher(AioIMDSFetcher, InstanceMetadataRegionFetcher):
     async def retrieve_region(self) -> Optional[str]: ...  # type: ignore [override]
 
+class AioS3RegionRedirectorv2(S3RegionRedirectorv2):
+    async def redirect_from_error(
+        self,
+        request_dict: Dict[str, Any],
+        response: Response,
+        operation: Any,
+        **kwargs: Any,
+    ) -> None: ...
+    async def get_bucket_region(self, bucket: Any, response: Response) -> Any: ...
+
 class AioS3RegionRedirector(S3RegionRedirector):
     async def redirect_from_error(
         self, request_dict: Dict[str, Any], response: Response, operation: Any, **kwargs: Any
     ) -> Optional[int]: ...
     async def get_bucket_region(self, bucket: str, response: Response) -> str: ...
 
 class AioContainerMetadataFetcher(ContainerMetadataFetcher):
```

### Comparing `types-aiobotocore-lite-2.5.2/aiobotocore-stubs/waiter.pyi` & `types-aiobotocore-lite-2.5.2.post1/aiobotocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lite-2.5.2/setup.py` & `types-aiobotocore-lite-2.5.2.post1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lite",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["aiobotocore-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.14.5",
+    description="Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.17.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
@@ -63,14 +63,15 @@
             "types-aiobotocore-amplifybackend>=2.5.0, <2.6.0",
             "types-aiobotocore-amplifyuibuilder>=2.5.0, <2.6.0",
             "types-aiobotocore-apigateway>=2.5.0, <2.6.0",
             "types-aiobotocore-apigatewaymanagementapi>=2.5.0, <2.6.0",
             "types-aiobotocore-apigatewayv2>=2.5.0, <2.6.0",
             "types-aiobotocore-appconfig>=2.5.0, <2.6.0",
             "types-aiobotocore-appconfigdata>=2.5.0, <2.6.0",
+            "types-aiobotocore-appfabric>=2.5.0, <2.6.0",
             "types-aiobotocore-appflow>=2.5.0, <2.6.0",
             "types-aiobotocore-appintegrations>=2.5.0, <2.6.0",
             "types-aiobotocore-application-autoscaling>=2.5.0, <2.6.0",
             "types-aiobotocore-application-insights>=2.5.0, <2.6.0",
             "types-aiobotocore-applicationcostprofiler>=2.5.0, <2.6.0",
             "types-aiobotocore-appmesh>=2.5.0, <2.6.0",
             "types-aiobotocore-apprunner>=2.5.0, <2.6.0",
@@ -166,14 +167,15 @@
             "types-aiobotocore-elasticbeanstalk>=2.5.0, <2.6.0",
             "types-aiobotocore-elastictranscoder>=2.5.0, <2.6.0",
             "types-aiobotocore-elb>=2.5.0, <2.6.0",
             "types-aiobotocore-elbv2>=2.5.0, <2.6.0",
             "types-aiobotocore-emr>=2.5.0, <2.6.0",
             "types-aiobotocore-emr-containers>=2.5.0, <2.6.0",
             "types-aiobotocore-emr-serverless>=2.5.0, <2.6.0",
+            "types-aiobotocore-entityresolution>=2.5.0, <2.6.0",
             "types-aiobotocore-es>=2.5.0, <2.6.0",
             "types-aiobotocore-events>=2.5.0, <2.6.0",
             "types-aiobotocore-evidently>=2.5.0, <2.6.0",
             "types-aiobotocore-finspace>=2.5.0, <2.6.0",
             "types-aiobotocore-finspace-data>=2.5.0, <2.6.0",
             "types-aiobotocore-firehose>=2.5.0, <2.6.0",
             "types-aiobotocore-fis>=2.5.0, <2.6.0",
@@ -252,26 +254,28 @@
             "types-aiobotocore-lookoutmetrics>=2.5.0, <2.6.0",
             "types-aiobotocore-lookoutvision>=2.5.0, <2.6.0",
             "types-aiobotocore-m2>=2.5.0, <2.6.0",
             "types-aiobotocore-machinelearning>=2.5.0, <2.6.0",
             "types-aiobotocore-macie>=2.5.0, <2.6.0",
             "types-aiobotocore-macie2>=2.5.0, <2.6.0",
             "types-aiobotocore-managedblockchain>=2.5.0, <2.6.0",
+            "types-aiobotocore-managedblockchain-query>=2.5.0, <2.6.0",
             "types-aiobotocore-marketplace-catalog>=2.5.0, <2.6.0",
             "types-aiobotocore-marketplace-entitlement>=2.5.0, <2.6.0",
             "types-aiobotocore-marketplacecommerceanalytics>=2.5.0, <2.6.0",
             "types-aiobotocore-mediaconnect>=2.5.0, <2.6.0",
             "types-aiobotocore-mediaconvert>=2.5.0, <2.6.0",
             "types-aiobotocore-medialive>=2.5.0, <2.6.0",
             "types-aiobotocore-mediapackage>=2.5.0, <2.6.0",
             "types-aiobotocore-mediapackage-vod>=2.5.0, <2.6.0",
             "types-aiobotocore-mediapackagev2>=2.5.0, <2.6.0",
             "types-aiobotocore-mediastore>=2.5.0, <2.6.0",
             "types-aiobotocore-mediastore-data>=2.5.0, <2.6.0",
             "types-aiobotocore-mediatailor>=2.5.0, <2.6.0",
+            "types-aiobotocore-medical-imaging>=2.5.0, <2.6.0",
             "types-aiobotocore-memorydb>=2.5.0, <2.6.0",
             "types-aiobotocore-meteringmarketplace>=2.5.0, <2.6.0",
             "types-aiobotocore-mgh>=2.5.0, <2.6.0",
             "types-aiobotocore-mgn>=2.5.0, <2.6.0",
             "types-aiobotocore-migration-hub-refactor-spaces>=2.5.0, <2.6.0",
             "types-aiobotocore-migrationhub-config>=2.5.0, <2.6.0",
             "types-aiobotocore-migrationhuborchestrator>=2.5.0, <2.6.0",
@@ -408,29 +412,30 @@
             "types-aiobotocore-dynamodb>=2.5.0, <2.6.0",
             "types-aiobotocore-ec2>=2.5.0, <2.6.0",
             "types-aiobotocore-lambda>=2.5.0, <2.6.0",
             "types-aiobotocore-rds>=2.5.0, <2.6.0",
             "types-aiobotocore-s3>=2.5.0, <2.6.0",
             "types-aiobotocore-sqs>=2.5.0, <2.6.0",
         ],
-        "aiobotocore": ["aiobotocore==2.5.2", "botocore==1.29.161"],
+        "aiobotocore": ["aiobotocore==2.5.2", "botocore==1.31.19"],
         "accessanalyzer": ["types-aiobotocore-accessanalyzer>=2.5.0, <2.6.0"],
         "account": ["types-aiobotocore-account>=2.5.0, <2.6.0"],
         "acm": ["types-aiobotocore-acm>=2.5.0, <2.6.0"],
         "acm-pca": ["types-aiobotocore-acm-pca>=2.5.0, <2.6.0"],
         "alexaforbusiness": ["types-aiobotocore-alexaforbusiness>=2.5.0, <2.6.0"],
         "amp": ["types-aiobotocore-amp>=2.5.0, <2.6.0"],
         "amplify": ["types-aiobotocore-amplify>=2.5.0, <2.6.0"],
         "amplifybackend": ["types-aiobotocore-amplifybackend>=2.5.0, <2.6.0"],
         "amplifyuibuilder": ["types-aiobotocore-amplifyuibuilder>=2.5.0, <2.6.0"],
         "apigateway": ["types-aiobotocore-apigateway>=2.5.0, <2.6.0"],
         "apigatewaymanagementapi": ["types-aiobotocore-apigatewaymanagementapi>=2.5.0, <2.6.0"],
         "apigatewayv2": ["types-aiobotocore-apigatewayv2>=2.5.0, <2.6.0"],
         "appconfig": ["types-aiobotocore-appconfig>=2.5.0, <2.6.0"],
         "appconfigdata": ["types-aiobotocore-appconfigdata>=2.5.0, <2.6.0"],
+        "appfabric": ["types-aiobotocore-appfabric>=2.5.0, <2.6.0"],
         "appflow": ["types-aiobotocore-appflow>=2.5.0, <2.6.0"],
         "appintegrations": ["types-aiobotocore-appintegrations>=2.5.0, <2.6.0"],
         "application-autoscaling": ["types-aiobotocore-application-autoscaling>=2.5.0, <2.6.0"],
         "application-insights": ["types-aiobotocore-application-insights>=2.5.0, <2.6.0"],
         "applicationcostprofiler": ["types-aiobotocore-applicationcostprofiler>=2.5.0, <2.6.0"],
         "appmesh": ["types-aiobotocore-appmesh>=2.5.0, <2.6.0"],
         "apprunner": ["types-aiobotocore-apprunner>=2.5.0, <2.6.0"],
@@ -526,14 +531,15 @@
         "elasticbeanstalk": ["types-aiobotocore-elasticbeanstalk>=2.5.0, <2.6.0"],
         "elastictranscoder": ["types-aiobotocore-elastictranscoder>=2.5.0, <2.6.0"],
         "elb": ["types-aiobotocore-elb>=2.5.0, <2.6.0"],
         "elbv2": ["types-aiobotocore-elbv2>=2.5.0, <2.6.0"],
         "emr": ["types-aiobotocore-emr>=2.5.0, <2.6.0"],
         "emr-containers": ["types-aiobotocore-emr-containers>=2.5.0, <2.6.0"],
         "emr-serverless": ["types-aiobotocore-emr-serverless>=2.5.0, <2.6.0"],
+        "entityresolution": ["types-aiobotocore-entityresolution>=2.5.0, <2.6.0"],
         "es": ["types-aiobotocore-es>=2.5.0, <2.6.0"],
         "events": ["types-aiobotocore-events>=2.5.0, <2.6.0"],
         "evidently": ["types-aiobotocore-evidently>=2.5.0, <2.6.0"],
         "finspace": ["types-aiobotocore-finspace>=2.5.0, <2.6.0"],
         "finspace-data": ["types-aiobotocore-finspace-data>=2.5.0, <2.6.0"],
         "firehose": ["types-aiobotocore-firehose>=2.5.0, <2.6.0"],
         "fis": ["types-aiobotocore-fis>=2.5.0, <2.6.0"],
@@ -620,28 +626,30 @@
         "lookoutmetrics": ["types-aiobotocore-lookoutmetrics>=2.5.0, <2.6.0"],
         "lookoutvision": ["types-aiobotocore-lookoutvision>=2.5.0, <2.6.0"],
         "m2": ["types-aiobotocore-m2>=2.5.0, <2.6.0"],
         "machinelearning": ["types-aiobotocore-machinelearning>=2.5.0, <2.6.0"],
         "macie": ["types-aiobotocore-macie>=2.5.0, <2.6.0"],
         "macie2": ["types-aiobotocore-macie2>=2.5.0, <2.6.0"],
         "managedblockchain": ["types-aiobotocore-managedblockchain>=2.5.0, <2.6.0"],
+        "managedblockchain-query": ["types-aiobotocore-managedblockchain-query>=2.5.0, <2.6.0"],
         "marketplace-catalog": ["types-aiobotocore-marketplace-catalog>=2.5.0, <2.6.0"],
         "marketplace-entitlement": ["types-aiobotocore-marketplace-entitlement>=2.5.0, <2.6.0"],
         "marketplacecommerceanalytics": [
             "types-aiobotocore-marketplacecommerceanalytics>=2.5.0, <2.6.0"
         ],
         "mediaconnect": ["types-aiobotocore-mediaconnect>=2.5.0, <2.6.0"],
         "mediaconvert": ["types-aiobotocore-mediaconvert>=2.5.0, <2.6.0"],
         "medialive": ["types-aiobotocore-medialive>=2.5.0, <2.6.0"],
         "mediapackage": ["types-aiobotocore-mediapackage>=2.5.0, <2.6.0"],
         "mediapackage-vod": ["types-aiobotocore-mediapackage-vod>=2.5.0, <2.6.0"],
         "mediapackagev2": ["types-aiobotocore-mediapackagev2>=2.5.0, <2.6.0"],
         "mediastore": ["types-aiobotocore-mediastore>=2.5.0, <2.6.0"],
         "mediastore-data": ["types-aiobotocore-mediastore-data>=2.5.0, <2.6.0"],
         "mediatailor": ["types-aiobotocore-mediatailor>=2.5.0, <2.6.0"],
+        "medical-imaging": ["types-aiobotocore-medical-imaging>=2.5.0, <2.6.0"],
         "memorydb": ["types-aiobotocore-memorydb>=2.5.0, <2.6.0"],
         "meteringmarketplace": ["types-aiobotocore-meteringmarketplace>=2.5.0, <2.6.0"],
         "mgh": ["types-aiobotocore-mgh>=2.5.0, <2.6.0"],
         "mgn": ["types-aiobotocore-mgn>=2.5.0, <2.6.0"],
         "migration-hub-refactor-spaces": [
             "types-aiobotocore-migration-hub-refactor-spaces>=2.5.0, <2.6.0"
         ],
```

### Comparing `types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/PKG-INFO` & `types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lite
-Version: 2.5.2
-Summary: Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore 2.5.2 generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -41,14 +41,15 @@
 Provides-Extra: amplifybackend
 Provides-Extra: amplifyuibuilder
 Provides-Extra: apigateway
 Provides-Extra: apigatewaymanagementapi
 Provides-Extra: apigatewayv2
 Provides-Extra: appconfig
 Provides-Extra: appconfigdata
+Provides-Extra: appfabric
 Provides-Extra: appflow
 Provides-Extra: appintegrations
 Provides-Extra: application-autoscaling
 Provides-Extra: application-insights
 Provides-Extra: applicationcostprofiler
 Provides-Extra: appmesh
 Provides-Extra: apprunner
@@ -144,14 +145,15 @@
 Provides-Extra: elasticbeanstalk
 Provides-Extra: elastictranscoder
 Provides-Extra: elb
 Provides-Extra: elbv2
 Provides-Extra: emr
 Provides-Extra: emr-containers
 Provides-Extra: emr-serverless
+Provides-Extra: entityresolution
 Provides-Extra: es
 Provides-Extra: events
 Provides-Extra: evidently
 Provides-Extra: finspace
 Provides-Extra: finspace-data
 Provides-Extra: firehose
 Provides-Extra: fis
@@ -230,26 +232,28 @@
 Provides-Extra: lookoutmetrics
 Provides-Extra: lookoutvision
 Provides-Extra: m2
 Provides-Extra: machinelearning
 Provides-Extra: macie
 Provides-Extra: macie2
 Provides-Extra: managedblockchain
+Provides-Extra: managedblockchain-query
 Provides-Extra: marketplace-catalog
 Provides-Extra: marketplace-entitlement
 Provides-Extra: marketplacecommerceanalytics
 Provides-Extra: mediaconnect
 Provides-Extra: mediaconvert
 Provides-Extra: medialive
 Provides-Extra: mediapackage
 Provides-Extra: mediapackage-vod
 Provides-Extra: mediapackagev2
 Provides-Extra: mediastore
 Provides-Extra: mediastore-data
 Provides-Extra: mediatailor
+Provides-Extra: medical-imaging
 Provides-Extra: memorydb
 Provides-Extra: meteringmarketplace
 Provides-Extra: mgh
 Provides-Extra: mgn
 Provides-Extra: migration-hub-refactor-spaces
 Provides-Extra: migrationhub-config
 Provides-Extra: migrationhuborchestrator
@@ -385,29 +389,29 @@
 <a id="types-aiobotocore-lite"></a>
 
 # types-aiobotocore-lite
 
 [![PyPI - types-aiobotocore-lite](https://img.shields.io/pypi/v/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lite.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lite)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lite?color=blue)](https://pypistats.org/packages/types-aiobotocore-lite)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lite)](https://pepy.tech/project/types-aiobotocore-lite)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore 2.5.2](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aiobotocore-lite docs](https://youtype.github.io/types_aiobotocore_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
@@ -678,15 +682,15 @@
 in [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder/issues/)
 repository.
 
 <a id="submodules"></a>
 
 ## Submodules
 
-- `types-aiobotocore-lite[all]` - Type annotations for all 349 services.
+- `types-aiobotocore-lite[all]` - Type annotations for all 353 services.
 - `types-aiobotocore-lite[essential]` - Type annotations for
   [CloudFormation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudformation/),
   [DynamoDB](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodb/),
   [EC2](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/),
   [Lambda](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/),
   [RDS](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rds/),
   [S3](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_s3/)
@@ -733,14 +737,17 @@
   service.
 - `types-aiobotocore-lite[appconfig]` - Type annotations for
   [AppConfig](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfig/)
   service.
 - `types-aiobotocore-lite[appconfigdata]` - Type annotations for
   [AppConfigData](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/)
   service.
+- `types-aiobotocore-lite[appfabric]` - Type annotations for
+  [AppFabric](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appfabric/)
+  service.
 - `types-aiobotocore-lite[appflow]` - Type annotations for
   [Appflow](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
   service.
 - `types-aiobotocore-lite[appintegrations]` - Type annotations for
   [AppIntegrationsService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/)
   service.
 - `types-aiobotocore-lite[application-autoscaling]` - Type annotations for
@@ -1042,14 +1049,17 @@
   service.
 - `types-aiobotocore-lite[emr-containers]` - Type annotations for
   [EMRContainers](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_containers/)
   service.
 - `types-aiobotocore-lite[emr-serverless]` - Type annotations for
   [EMRServerless](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_emr_serverless/)
   service.
+- `types-aiobotocore-lite[entityresolution]` - Type annotations for
+  [EntityResolution](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_entityresolution/)
+  service.
 - `types-aiobotocore-lite[es]` - Type annotations for
   [ElasticsearchService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es/)
   service.
 - `types-aiobotocore-lite[events]` - Type annotations for
   [EventBridge](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
   service.
 - `types-aiobotocore-lite[evidently]` - Type annotations for
@@ -1302,14 +1312,17 @@
   service.
 - `types-aiobotocore-lite[macie2]` - Type annotations for
   [Macie2](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
   service.
 - `types-aiobotocore-lite[managedblockchain]` - Type annotations for
   [ManagedBlockchain](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
   service.
+- `types-aiobotocore-lite[managedblockchain-query]` - Type annotations for
+  [ManagedBlockchainQuery](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain_query/)
+  service.
 - `types-aiobotocore-lite[marketplace-catalog]` - Type annotations for
   [MarketplaceCatalog](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
   service.
 - `types-aiobotocore-lite[marketplace-entitlement]` - Type annotations for
   [MarketplaceEntitlementService](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
   service.
 - `types-aiobotocore-lite[marketplacecommerceanalytics]` - Type annotations for
@@ -1338,14 +1351,17 @@
   service.
 - `types-aiobotocore-lite[mediastore-data]` - Type annotations for
   [MediaStoreData](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediastore_data/)
   service.
 - `types-aiobotocore-lite[mediatailor]` - Type annotations for
   [MediaTailor](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/)
   service.
+- `types-aiobotocore-lite[medical-imaging]` - Type annotations for
+  [HealthImaging](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_medical_imaging/)
+  service.
 - `types-aiobotocore-lite[memorydb]` - Type annotations for
   [MemoryDB](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/)
   service.
 - `types-aiobotocore-lite[meteringmarketplace]` - Type annotations for
   [MarketplaceMetering](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_meteringmarketplace/)
   service.
 - `types-aiobotocore-lite[mgh]` - Type annotations for
```

### Comparing `types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/SOURCES.txt` & `types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 aiobotocore-stubs/handlers.pyi
 aiobotocore-stubs/hooks.pyi
 aiobotocore-stubs/httpchecksum.pyi
 aiobotocore-stubs/httpsession.pyi
 aiobotocore-stubs/paginate.pyi
 aiobotocore-stubs/parsers.pyi
 aiobotocore-stubs/py.typed
+aiobotocore-stubs/regions.pyi
 aiobotocore-stubs/response.pyi
 aiobotocore-stubs/retryhandler.pyi
 aiobotocore-stubs/session.pyi
 aiobotocore-stubs/signers.pyi
+aiobotocore-stubs/tokens.pyi
 aiobotocore-stubs/utils.pyi
-aiobotocore-stubs/version.py
 aiobotocore-stubs/waiter.pyi
 types_aiobotocore_lite.egg-info/PKG-INFO
 types_aiobotocore_lite.egg-info/SOURCES.txt
 types_aiobotocore_lite.egg-info/dependency_links.txt
 types_aiobotocore_lite.egg-info/not-zip-safe
 types_aiobotocore_lite.egg-info/requires.txt
 types_aiobotocore_lite.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lite-2.5.2/types_aiobotocore_lite.egg-info/requires.txt` & `types-aiobotocore-lite-2.5.2.post1/types_aiobotocore_lite.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 types-aiobotocore-acm<2.6.0,>=2.5.0
 
 [acm-pca]
 types-aiobotocore-acm-pca<2.6.0,>=2.5.0
 
 [aiobotocore]
 aiobotocore==2.5.2
-botocore==1.29.161
+botocore==1.31.19
 
 [alexaforbusiness]
 types-aiobotocore-alexaforbusiness<2.6.0,>=2.5.0
 
 [all]
 types-aiobotocore-accessanalyzer<2.6.0,>=2.5.0
 types-aiobotocore-account<2.6.0,>=2.5.0
@@ -33,14 +33,15 @@
 types-aiobotocore-amplifybackend<2.6.0,>=2.5.0
 types-aiobotocore-amplifyuibuilder<2.6.0,>=2.5.0
 types-aiobotocore-apigateway<2.6.0,>=2.5.0
 types-aiobotocore-apigatewaymanagementapi<2.6.0,>=2.5.0
 types-aiobotocore-apigatewayv2<2.6.0,>=2.5.0
 types-aiobotocore-appconfig<2.6.0,>=2.5.0
 types-aiobotocore-appconfigdata<2.6.0,>=2.5.0
+types-aiobotocore-appfabric<2.6.0,>=2.5.0
 types-aiobotocore-appflow<2.6.0,>=2.5.0
 types-aiobotocore-appintegrations<2.6.0,>=2.5.0
 types-aiobotocore-application-autoscaling<2.6.0,>=2.5.0
 types-aiobotocore-application-insights<2.6.0,>=2.5.0
 types-aiobotocore-applicationcostprofiler<2.6.0,>=2.5.0
 types-aiobotocore-appmesh<2.6.0,>=2.5.0
 types-aiobotocore-apprunner<2.6.0,>=2.5.0
@@ -136,14 +137,15 @@
 types-aiobotocore-elasticbeanstalk<2.6.0,>=2.5.0
 types-aiobotocore-elastictranscoder<2.6.0,>=2.5.0
 types-aiobotocore-elb<2.6.0,>=2.5.0
 types-aiobotocore-elbv2<2.6.0,>=2.5.0
 types-aiobotocore-emr<2.6.0,>=2.5.0
 types-aiobotocore-emr-containers<2.6.0,>=2.5.0
 types-aiobotocore-emr-serverless<2.6.0,>=2.5.0
+types-aiobotocore-entityresolution<2.6.0,>=2.5.0
 types-aiobotocore-es<2.6.0,>=2.5.0
 types-aiobotocore-events<2.6.0,>=2.5.0
 types-aiobotocore-evidently<2.6.0,>=2.5.0
 types-aiobotocore-finspace<2.6.0,>=2.5.0
 types-aiobotocore-finspace-data<2.6.0,>=2.5.0
 types-aiobotocore-firehose<2.6.0,>=2.5.0
 types-aiobotocore-fis<2.6.0,>=2.5.0
@@ -222,26 +224,28 @@
 types-aiobotocore-lookoutmetrics<2.6.0,>=2.5.0
 types-aiobotocore-lookoutvision<2.6.0,>=2.5.0
 types-aiobotocore-m2<2.6.0,>=2.5.0
 types-aiobotocore-machinelearning<2.6.0,>=2.5.0
 types-aiobotocore-macie<2.6.0,>=2.5.0
 types-aiobotocore-macie2<2.6.0,>=2.5.0
 types-aiobotocore-managedblockchain<2.6.0,>=2.5.0
+types-aiobotocore-managedblockchain-query<2.6.0,>=2.5.0
 types-aiobotocore-marketplace-catalog<2.6.0,>=2.5.0
 types-aiobotocore-marketplace-entitlement<2.6.0,>=2.5.0
 types-aiobotocore-marketplacecommerceanalytics<2.6.0,>=2.5.0
 types-aiobotocore-mediaconnect<2.6.0,>=2.5.0
 types-aiobotocore-mediaconvert<2.6.0,>=2.5.0
 types-aiobotocore-medialive<2.6.0,>=2.5.0
 types-aiobotocore-mediapackage<2.6.0,>=2.5.0
 types-aiobotocore-mediapackage-vod<2.6.0,>=2.5.0
 types-aiobotocore-mediapackagev2<2.6.0,>=2.5.0
 types-aiobotocore-mediastore<2.6.0,>=2.5.0
 types-aiobotocore-mediastore-data<2.6.0,>=2.5.0
 types-aiobotocore-mediatailor<2.6.0,>=2.5.0
+types-aiobotocore-medical-imaging<2.6.0,>=2.5.0
 types-aiobotocore-memorydb<2.6.0,>=2.5.0
 types-aiobotocore-meteringmarketplace<2.6.0,>=2.5.0
 types-aiobotocore-mgh<2.6.0,>=2.5.0
 types-aiobotocore-mgn<2.6.0,>=2.5.0
 types-aiobotocore-migration-hub-refactor-spaces<2.6.0,>=2.5.0
 types-aiobotocore-migrationhub-config<2.6.0,>=2.5.0
 types-aiobotocore-migrationhuborchestrator<2.6.0,>=2.5.0
@@ -396,14 +400,17 @@
 
 [appconfig]
 types-aiobotocore-appconfig<2.6.0,>=2.5.0
 
 [appconfigdata]
 types-aiobotocore-appconfigdata<2.6.0,>=2.5.0
 
+[appfabric]
+types-aiobotocore-appfabric<2.6.0,>=2.5.0
+
 [appflow]
 types-aiobotocore-appflow<2.6.0,>=2.5.0
 
 [appintegrations]
 types-aiobotocore-appintegrations<2.6.0,>=2.5.0
 
 [application-autoscaling]
@@ -705,14 +712,17 @@
 
 [emr-containers]
 types-aiobotocore-emr-containers<2.6.0,>=2.5.0
 
 [emr-serverless]
 types-aiobotocore-emr-serverless<2.6.0,>=2.5.0
 
+[entityresolution]
+types-aiobotocore-entityresolution<2.6.0,>=2.5.0
+
 [es]
 types-aiobotocore-es<2.6.0,>=2.5.0
 
 [essential]
 types-aiobotocore-cloudformation<2.6.0,>=2.5.0
 types-aiobotocore-dynamodb<2.6.0,>=2.5.0
 types-aiobotocore-ec2<2.6.0,>=2.5.0
@@ -972,14 +982,17 @@
 
 [macie2]
 types-aiobotocore-macie2<2.6.0,>=2.5.0
 
 [managedblockchain]
 types-aiobotocore-managedblockchain<2.6.0,>=2.5.0
 
+[managedblockchain-query]
+types-aiobotocore-managedblockchain-query<2.6.0,>=2.5.0
+
 [marketplace-catalog]
 types-aiobotocore-marketplace-catalog<2.6.0,>=2.5.0
 
 [marketplace-entitlement]
 types-aiobotocore-marketplace-entitlement<2.6.0,>=2.5.0
 
 [marketplacecommerceanalytics]
@@ -1008,14 +1021,17 @@
 
 [mediastore-data]
 types-aiobotocore-mediastore-data<2.6.0,>=2.5.0
 
 [mediatailor]
 types-aiobotocore-mediatailor<2.6.0,>=2.5.0
 
+[medical-imaging]
+types-aiobotocore-medical-imaging<2.6.0,>=2.5.0
+
 [memorydb]
 types-aiobotocore-memorydb<2.6.0,>=2.5.0
 
 [meteringmarketplace]
 types-aiobotocore-meteringmarketplace<2.6.0,>=2.5.0
 
 [mgh]
```

