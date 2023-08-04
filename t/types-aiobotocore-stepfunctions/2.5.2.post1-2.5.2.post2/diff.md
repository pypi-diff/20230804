# Comparing `tmp/types-aiobotocore-stepfunctions-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-stepfunctions-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-stepfunctions-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-stepfunctions-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-stepfunctions-2.5.2.post1.tar` & `types-aiobotocore-stepfunctions-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.513444 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30297 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44359 2023-08-02 14:50:21.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44294 2023-08-02 14:50:20.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:19.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.521444 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18513 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:53:05.000000 types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13736 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12204 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2104 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1465 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1464 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    30282 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    30234 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10946 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10944 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6689 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6682 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43905 2023-08-04 13:54:37.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43840 2023-08-04 13:54:36.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:35.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.306643 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13736 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:28.000000 types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/LICENSE` & `types-aiobotocore-stepfunctions-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/setup.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-stepfunctions",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SFN 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__init__.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/__main__.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SFN 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SFN 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationUnionTypeDef,
+    LoggingConfigurationTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
@@ -153,15 +153,15 @@
     async def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -511,15 +511,15 @@
 
     async def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/client.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
     ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    LoggingConfigurationUnionTypeDef,
+    LoggingConfigurationTypeDef,
     PublishStateMachineVersionOutputTypeDef,
     RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
@@ -145,15 +145,15 @@
     async def create_state_machine(
         self,
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
-        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
@@ -471,15 +471,15 @@
         """
     async def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
-        loggingConfiguration: LoggingConfigurationUnionTypeDef = ...,
+        loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
         versionDescription: str = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -227,14 +228,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -313,26 +315,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -500,14 +504,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/literals.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -225,14 +226,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -311,26 +313,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
@@ -498,14 +502,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/paginator.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.py` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_stepfunctions.type_defs import ActivityFailedEventDetailsTypeDef
 
     data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ExecutionStatusType,
     HistoryEventTypeType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
@@ -136,21 +136,19 @@
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -1546,24 +1544,14 @@
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingConfigurationOutputTypeDef = TypedDict(
-    "LoggingConfigurationOutputTypeDef",
-    {
-        "level": LogLevelType,
-        "includeExecutionData": bool,
-        "destinations": List[LogDestinationTypeDef],
-    },
-    total=False,
-)
-
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
         "destinations": Sequence[LogDestinationTypeDef],
     },
@@ -1621,23 +1609,51 @@
 )
 
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
 
+_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+    },
+)
+_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineInputRequestTypeDef",
+    {
+        "type": StateMachineTypeType,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
+    },
+    total=False,
+)
+
+
+class CreateStateMachineInputRequestTypeDef(
+    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
+):
+    pass
+
+
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1648,54 +1664,23 @@
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineInputRequestTypeDef",
-    {
-        "type": StateMachineTypeType,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
-    },
-    total=False,
-)
-
-
-class CreateStateMachineInputRequestTypeDef(
-    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
-):
-    pass
-
-
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions/type_defs.pyi` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_stepfunctions.type_defs import ActivityFailedEventDetailsTypeDef
 
     data: ActivityFailedEventDetailsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ExecutionStatusType,
     HistoryEventTypeType,
     LogLevelType,
     MapRunStatusType,
     StateMachineStatusType,
@@ -135,21 +135,19 @@
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
     "ListStateMachineAliasesOutputTypeDef",
     "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
-    "LoggingConfigurationOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
+    "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
-    "CreateStateMachineInputRequestTypeDef",
-    "LoggingConfigurationUnionTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
     "GetExecutionHistoryOutputTypeDef",
 )
 
 ActivityFailedEventDetailsTypeDef = TypedDict(
     "ActivityFailedEventDetailsTypeDef",
     {
@@ -1487,24 +1485,14 @@
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingConfigurationOutputTypeDef = TypedDict(
-    "LoggingConfigurationOutputTypeDef",
-    {
-        "level": LogLevelType,
-        "includeExecutionData": bool,
-        "destinations": List[LogDestinationTypeDef],
-    },
-    total=False,
-)
-
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "level": LogLevelType,
         "includeExecutionData": bool,
         "destinations": Sequence[LogDestinationTypeDef],
     },
@@ -1560,23 +1548,49 @@
     },
     total=False,
 )
 
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
+_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_RequiredCreateStateMachineInputRequestTypeDef",
+    {
+        "name": str,
+        "definition": str,
+        "roleArn": str,
+    },
+)
+_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
+    "_OptionalCreateStateMachineInputRequestTypeDef",
+    {
+        "type": StateMachineTypeType,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "tracingConfiguration": TracingConfigurationTypeDef,
+        "publish": bool,
+        "versionDescription": str,
+    },
+    total=False,
+)
+
+class CreateStateMachineInputRequestTypeDef(
+    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
+):
+    pass
+
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
-        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
         "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1587,52 +1601,23 @@
         "stateMachineArn": str,
         "name": str,
         "status": StateMachineStatusType,
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
-        "loggingConfiguration": LoggingConfigurationOutputTypeDef,
+        "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
         "revisionId": str,
         "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineInputRequestTypeDef",
-    {
-        "name": str,
-        "definition": str,
-        "roleArn": str,
-    },
-)
-_OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineInputRequestTypeDef",
-    {
-        "type": StateMachineTypeType,
-        "loggingConfiguration": LoggingConfigurationTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
-    },
-    total=False,
-)
-
-class CreateStateMachineInputRequestTypeDef(
-    _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
-):
-    pass
-
-LoggingConfigurationUnionTypeDef = Union[
-    LoggingConfigurationTypeDef, LoggingConfigurationOutputTypeDef
-]
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-stepfunctions-2.5.2.post1/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt` & `types-aiobotocore-stepfunctions-2.5.2.post2/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

