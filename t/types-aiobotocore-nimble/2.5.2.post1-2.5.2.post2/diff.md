# Comparing `tmp/types-aiobotocore-nimble-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-nimble-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-nimble-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-nimble-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:19 2023, max compression
```

## Comparing `types-aiobotocore-nimble-2.5.2.post1.tar` & `types-aiobotocore-nimble-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.429511 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47158 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47078 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18079 2023-08-02 14:44:10.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    18077 2023-08-02 14:44:09.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    71705 2023-08-02 14:44:11.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    71586 2023-08-02 14:44:10.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:06.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-08-02 14:44:07.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.437511 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25272 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:43.000000 types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16801 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15281 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2071 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5224 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5223 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      940 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47143 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47063 2023-08-04 13:45:44.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18174 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    18172 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12886 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12874 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    70018 2023-08-04 13:45:47.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    69901 2023-08-04 13:45:46.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:43.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13016 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13004 2023-08-04 13:45:45.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:19.616643 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16801 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      865 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:19.000000 types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/LICENSE` & `types-aiobotocore-nimble-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/setup.py` & `types-aiobotocore-nimble-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-nimble",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_nimble"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.NimbleStudio 2.5.2 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__init__.pyi` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/__main__.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NimbleStudio 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.NimbleStudio 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_nimble//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio\nOther"
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

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
-    StudioComponentConfigurationUnionTypeDef,
+    StudioComponentConfigurationTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     UpdateStudioResponseTypeDef,
@@ -269,15 +269,15 @@
     async def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationUnionTypeDef = ...,
+        configuration: StudioComponentConfigurationTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -777,15 +777,15 @@
 
     async def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationUnionTypeDef = ...,
+        configuration: StudioComponentConfigurationTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/client.pyi` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     NewLaunchProfileMemberTypeDef,
     NewStudioMemberTypeDef,
     ScriptParameterKeyValueTypeDef,
     StartStreamingSessionResponseTypeDef,
     StartStudioSSOConfigurationRepairResponseTypeDef,
     StopStreamingSessionResponseTypeDef,
     StreamConfigurationCreateTypeDef,
-    StudioComponentConfigurationUnionTypeDef,
+    StudioComponentConfigurationTypeDef,
     StudioComponentInitializationScriptTypeDef,
     StudioEncryptionConfigurationTypeDef,
     UpdateLaunchProfileMemberResponseTypeDef,
     UpdateLaunchProfileResponseTypeDef,
     UpdateStreamingImageResponseTypeDef,
     UpdateStudioComponentResponseTypeDef,
     UpdateStudioResponseTypeDef,
@@ -256,15 +256,15 @@
     async def create_studio_component(
         self,
         *,
         name: str,
         studioId: str,
         type: StudioComponentTypeType,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationUnionTypeDef = ...,
+        configuration: StudioComponentConfigurationTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
         subtype: StudioComponentSubtypeType = ...,
@@ -721,15 +721,15 @@
         """
     async def update_studio_component(
         self,
         *,
         studioComponentId: str,
         studioId: str,
         clientToken: str = ...,
-        configuration: StudioComponentConfigurationUnionTypeDef = ...,
+        configuration: StudioComponentConfigurationTypeDef = ...,
         description: str = ...,
         ec2SecurityGroupIds: Sequence[str] = ...,
         initializationScripts: Sequence[StudioComponentInitializationScriptTypeDef] = ...,
         name: str = ...,
         runtimeRoleArn: str = ...,
         scriptParameters: Sequence[ScriptParameterKeyValueTypeDef] = ...,
         secureInitializationRoleArn: str = ...,
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,14 +315,15 @@
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
@@ -418,14 +419,15 @@
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
@@ -504,26 +506,28 @@
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
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/literals.pyi` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -313,14 +313,15 @@
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
@@ -416,14 +417,15 @@
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
@@ -502,26 +504,28 @@
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
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/paginator.pyi` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_nimble.type_defs import AcceptEulasRequestRequestTypeDef
 
     data: AcceptEulasRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AutomaticTerminationModeType,
     LaunchProfilePlatformType,
     LaunchProfileStateType,
     LaunchProfileStatusCodeType,
     LaunchProfileValidationStateType,
@@ -49,15 +49,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
     "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
@@ -121,15 +120,14 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateLaunchProfileMemberRequestRequestTypeDef",
     "UpdateStreamingImageRequestRequestTypeDef",
     "UpdateStudioRequestRequestTypeDef",
     "AcceptEulasResponseTypeDef",
     "ListEulaAcceptancesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ActiveDirectoryConfigurationOutputTypeDef",
     "ActiveDirectoryConfigurationTypeDef",
     "LaunchProfileInitializationActiveDirectoryTypeDef",
     "CreateStreamingSessionStreamResponseTypeDef",
     "GetStreamingSessionStreamResponseTypeDef",
     "CreateStudioRequestRequestTypeDef",
     "StudioTypeDef",
     "GetEulaResponseTypeDef",
@@ -162,47 +160,44 @@
     "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
     "ListStudiosRequestListStudiosPaginateTypeDef",
     "PutLaunchProfileMembersRequestRequestTypeDef",
     "PutStudioMembersRequestRequestTypeDef",
     "StreamingSessionTypeDef",
-    "StreamConfigurationSessionStorageOutputTypeDef",
     "StreamConfigurationSessionStorageTypeDef",
     "StreamingImageTypeDef",
-    "StudioComponentConfigurationOutputTypeDef",
     "StudioComponentConfigurationTypeDef",
     "LaunchProfileInitializationTypeDef",
     "CreateStudioResponseTypeDef",
     "DeleteStudioResponseTypeDef",
     "GetStudioResponseTypeDef",
     "ListStudiosResponseTypeDef",
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     "UpdateStudioResponseTypeDef",
     "CreateStreamingSessionResponseTypeDef",
     "DeleteStreamingSessionResponseTypeDef",
     "GetStreamingSessionResponseTypeDef",
     "ListStreamingSessionsResponseTypeDef",
     "StartStreamingSessionResponseTypeDef",
     "StopStreamingSessionResponseTypeDef",
-    "StreamConfigurationTypeDef",
     "StreamConfigurationCreateTypeDef",
+    "StreamConfigurationTypeDef",
     "CreateStreamingImageResponseTypeDef",
     "DeleteStreamingImageResponseTypeDef",
     "GetStreamingImageResponseTypeDef",
     "ListStreamingImagesResponseTypeDef",
     "UpdateStreamingImageResponseTypeDef",
-    "StudioComponentTypeDef",
     "CreateStudioComponentRequestRequestTypeDef",
-    "StudioComponentConfigurationUnionTypeDef",
+    "StudioComponentTypeDef",
     "UpdateStudioComponentRequestRequestTypeDef",
     "GetLaunchProfileInitializationResponseTypeDef",
-    "LaunchProfileTypeDef",
     "CreateLaunchProfileRequestRequestTypeDef",
     "UpdateLaunchProfileRequestRequestTypeDef",
+    "LaunchProfileTypeDef",
     "CreateStudioComponentResponseTypeDef",
     "DeleteStudioComponentResponseTypeDef",
     "GetStudioComponentResponseTypeDef",
     "ListStudioComponentsResponseTypeDef",
     "UpdateStudioComponentResponseTypeDef",
     "CreateLaunchProfileResponseTypeDef",
     "DeleteLaunchProfileResponseTypeDef",
@@ -223,21 +218,19 @@
     {
         "clientToken": str,
         "eulaIds": Sequence[str],
     },
     total=False,
 )
 
-
 class AcceptEulasRequestRequestTypeDef(
     _RequiredAcceptEulasRequestRequestTypeDef, _OptionalAcceptEulasRequestRequestTypeDef
 ):
     pass
 
-
 EulaAcceptanceTypeDef = TypedDict(
     "EulaAcceptanceTypeDef",
     {
         "acceptedAt": datetime,
         "acceptedBy": str,
         "accepteeId": str,
         "eulaAcceptanceId": str,
@@ -289,22 +282,20 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStreamingImageRequestRequestTypeDef(
     _RequiredCreateStreamingImageRequestRequestTypeDef,
     _OptionalCreateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -316,22 +307,20 @@
         "ownedBy": str,
         "streamingImageId": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStreamingSessionRequestRequestTypeDef(
     _RequiredCreateStreamingSessionRequestRequestTypeDef,
     _OptionalCreateStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateStreamingSessionStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionStreamRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -340,22 +329,20 @@
     {
         "clientToken": str,
         "expirationInSeconds": int,
     },
     total=False,
 )
 
-
 class CreateStreamingSessionStreamRequestRequestTypeDef(
     _RequiredCreateStreamingSessionStreamRequestRequestTypeDef,
     _OptionalCreateStreamingSessionStreamRequestRequestTypeDef,
 ):
     pass
 
-
 StreamingSessionStreamTypeDef = TypedDict(
     "StreamingSessionStreamTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "expiresAt": datetime,
         "ownedBy": str,
@@ -397,21 +384,19 @@
     "_OptionalStudioEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
-
 class StudioEncryptionConfigurationTypeDef(
     _RequiredStudioEncryptionConfigurationTypeDef, _OptionalStudioEncryptionConfigurationTypeDef
 ):
     pass
 
-
 _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "principalId": str,
         "studioId": str,
     },
@@ -420,22 +405,20 @@
     "_OptionalDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteLaunchProfileMemberRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -443,22 +426,20 @@
     "_OptionalDeleteLaunchProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteLaunchProfileRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -466,22 +447,20 @@
     "_OptionalDeleteStreamingImageRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStreamingImageRequestRequestTypeDef(
     _RequiredDeleteStreamingImageRequestRequestTypeDef,
     _OptionalDeleteStreamingImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -489,22 +468,20 @@
     "_OptionalDeleteStreamingSessionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStreamingSessionRequestRequestTypeDef(
     _RequiredDeleteStreamingSessionRequestRequestTypeDef,
     _OptionalDeleteStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -512,22 +489,20 @@
     "_OptionalDeleteStudioComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStudioComponentRequestRequestTypeDef(
     _RequiredDeleteStudioComponentRequestRequestTypeDef,
     _OptionalDeleteStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStudioMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioMemberRequestRequestTypeDef",
     {
         "principalId": str,
         "studioId": str,
     },
 )
@@ -535,43 +510,39 @@
     "_OptionalDeleteStudioMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStudioMemberRequestRequestTypeDef(
     _RequiredDeleteStudioMemberRequestRequestTypeDef,
     _OptionalDeleteStudioMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteStudioRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalDeleteStudioRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStudioRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class DeleteStudioRequestRequestTypeDef(
     _RequiredDeleteStudioRequestRequestTypeDef, _OptionalDeleteStudioRequestRequestTypeDef
 ):
     pass
 
-
 EulaTypeDef = TypedDict(
     "EulaTypeDef",
     {
         "content": str,
         "createdAt": datetime,
         "eulaId": str,
         "name": str,
@@ -794,22 +765,20 @@
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListEulaAcceptancesRequestRequestTypeDef(
     _RequiredListEulaAcceptancesRequestRequestTypeDef,
     _OptionalListEulaAcceptancesRequestRequestTypeDef,
 ):
     pass
 
-
 ListEulasRequestRequestTypeDef = TypedDict(
     "ListEulasRequestRequestTypeDef",
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
@@ -827,22 +796,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListLaunchProfileMembersRequestRequestTypeDef(
     _RequiredListLaunchProfileMembersRequestRequestTypeDef,
     _OptionalListLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLaunchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestRequestTypeDef = TypedDict(
@@ -852,22 +819,20 @@
         "nextToken": str,
         "principalId": str,
         "states": Sequence[LaunchProfileStateType],
     },
     total=False,
 )
 
-
 class ListLaunchProfilesRequestRequestTypeDef(
     _RequiredListLaunchProfilesRequestRequestTypeDef,
     _OptionalListLaunchProfilesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListStreamingImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestRequestTypeDef = TypedDict(
@@ -875,22 +840,20 @@
     {
         "nextToken": str,
         "owner": str,
     },
     total=False,
 )
 
-
 class ListStreamingImagesRequestRequestTypeDef(
     _RequiredListStreamingImagesRequestRequestTypeDef,
     _OptionalListStreamingImagesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
@@ -898,22 +861,20 @@
     {
         "nextToken": str,
         "ownedBy": str,
     },
     total=False,
 )
 
-
 class ListStreamingSessionBackupsRequestRequestTypeDef(
     _RequiredListStreamingSessionBackupsRequestRequestTypeDef,
     _OptionalListStreamingSessionBackupsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListStreamingSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestRequestTypeDef = TypedDict(
@@ -923,22 +884,20 @@
         "nextToken": str,
         "ownedBy": str,
         "sessionIds": str,
     },
     total=False,
 )
 
-
 class ListStreamingSessionsRequestRequestTypeDef(
     _RequiredListStreamingSessionsRequestRequestTypeDef,
     _OptionalListStreamingSessionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListStudioComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestRequestTypeDef = TypedDict(
@@ -948,22 +907,20 @@
         "nextToken": str,
         "states": Sequence[StudioComponentStateType],
         "types": Sequence[StudioComponentTypeType],
     },
     total=False,
 )
 
-
 class ListStudioComponentsRequestRequestTypeDef(
     _RequiredListStudioComponentsRequestRequestTypeDef,
     _OptionalListStudioComponentsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestRequestTypeDef = TypedDict(
@@ -971,21 +928,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListStudioMembersRequestRequestTypeDef(
     _RequiredListStudioMembersRequestRequestTypeDef, _OptionalListStudioMembersRequestRequestTypeDef
 ):
     pass
 
-
 ListStudiosRequestRequestTypeDef = TypedDict(
     "ListStudiosRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1037,44 +992,40 @@
     {
         "backupId": str,
         "clientToken": str,
     },
     total=False,
 )
 
-
 class StartStreamingSessionRequestRequestTypeDef(
     _RequiredStartStreamingSessionRequestRequestTypeDef,
     _OptionalStartStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class StartStudioSSOConfigurationRepairRequestRequestTypeDef(
     _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef,
     _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredStopStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStopStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1083,22 +1034,20 @@
     {
         "clientToken": str,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
-
 class StopStreamingSessionRequestRequestTypeDef(
     _RequiredStopStreamingSessionRequestRequestTypeDef,
     _OptionalStopStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
-
 StreamConfigurationSessionBackupTypeDef = TypedDict(
     "StreamConfigurationSessionBackupTypeDef",
     {
         "maxBackupsToRetain": int,
         "mode": SessionBackupModeType,
     },
     total=False,
@@ -1133,43 +1082,39 @@
     "_OptionalStreamingImageEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
-
 class StreamingImageEncryptionConfigurationTypeDef(
     _RequiredStreamingImageEncryptionConfigurationTypeDef,
     _OptionalStreamingImageEncryptionConfigurationTypeDef,
 ):
     pass
 
-
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1187,22 +1132,20 @@
     "_OptionalUpdateLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class UpdateLaunchProfileMemberRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileMemberRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1212,22 +1155,20 @@
         "clientToken": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
-
 class UpdateStreamingImageRequestRequestTypeDef(
     _RequiredUpdateStreamingImageRequestRequestTypeDef,
     _OptionalUpdateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalUpdateStudioRequestRequestTypeDef = TypedDict(
@@ -1237,21 +1178,19 @@
         "clientToken": str,
         "displayName": str,
         "userRoleArn": str,
     },
     total=False,
 )
 
-
 class UpdateStudioRequestRequestTypeDef(
     _RequiredUpdateStudioRequestRequestTypeDef, _OptionalUpdateStudioRequestRequestTypeDef
 ):
     pass
 
-
 AcceptEulasResponseTypeDef = TypedDict(
     "AcceptEulasResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1269,24 +1208,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActiveDirectoryConfigurationOutputTypeDef = TypedDict(
-    "ActiveDirectoryConfigurationOutputTypeDef",
-    {
-        "computerAttributes": List[ActiveDirectoryComputerAttributeTypeDef],
-        "directoryId": str,
-        "organizationalUnitDistinguishedName": str,
-    },
-    total=False,
-)
-
 ActiveDirectoryConfigurationTypeDef = TypedDict(
     "ActiveDirectoryConfigurationTypeDef",
     {
         "computerAttributes": Sequence[ActiveDirectoryComputerAttributeTypeDef],
         "directoryId": str,
         "organizationalUnitDistinguishedName": str,
     },
@@ -1338,21 +1267,19 @@
         "clientToken": str,
         "studioEncryptionConfiguration": StudioEncryptionConfigurationTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStudioRequestRequestTypeDef(
     _RequiredCreateStudioRequestRequestTypeDef, _OptionalCreateStudioRequestRequestTypeDef
 ):
     pass
 
-
 StudioTypeDef = TypedDict(
     "StudioTypeDef",
     {
         "adminRoleArn": str,
         "arn": str,
         "createdAt": datetime,
         "displayName": str,
@@ -1425,22 +1352,20 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -1448,22 +1373,20 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1471,22 +1394,20 @@
     "_OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingImageRequestStreamingImageDeletedWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1494,22 +1415,20 @@
     "_OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingImageRequestStreamingImageReadyWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1517,22 +1436,20 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1540,22 +1457,20 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1563,22 +1478,20 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "sessionId": str,
         "streamId": str,
         "studioId": str,
     },
@@ -1587,22 +1500,20 @@
     "_OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef(
     _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
     _OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1610,22 +1521,20 @@
     "_OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioComponentRequestStudioComponentDeletedWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1633,65 +1542,59 @@
     "_OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioComponentRequestStudioComponentReadyWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioRequestStudioDeletedWaitTypeDef(
     _RequiredGetStudioRequestStudioDeletedWaitTypeDef,
     _OptionalGetStudioRequestStudioDeletedWaitTypeDef,
 ):
     pass
 
-
 _RequiredGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioReadyWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetStudioRequestStudioReadyWaitTypeDef(
     _RequiredGetStudioRequestStudioReadyWaitTypeDef, _OptionalGetStudioRequestStudioReadyWaitTypeDef
 ):
     pass
 
-
 GetStreamingSessionBackupResponseTypeDef = TypedDict(
     "GetStreamingSessionBackupResponseTypeDef",
     {
         "streamingSessionBackup": StreamingSessionBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1733,22 +1636,20 @@
     {
         "eulaIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
     _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
     _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
 ):
     pass
 
-
 ListEulasRequestListEulasPaginateTypeDef = TypedDict(
     "ListEulasRequestListEulasPaginateTypeDef",
     {
         "eulaIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1765,22 +1666,20 @@
     "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
     _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
@@ -1789,22 +1688,20 @@
         "principalId": str,
         "states": Sequence[LaunchProfileStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
     _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
@@ -1812,22 +1709,20 @@
     {
         "owner": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
     _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
@@ -1835,22 +1730,20 @@
     {
         "ownedBy": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
     _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
@@ -1860,22 +1753,20 @@
         "ownedBy": str,
         "sessionIds": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
     _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
@@ -1884,44 +1775,40 @@
         "states": Sequence[StudioComponentStateType],
         "types": Sequence[StudioComponentTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
     _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
     "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
     _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
     _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
 ):
     pass
 
-
 ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
     "ListStudiosRequestListStudiosPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1939,22 +1826,20 @@
     "_OptionalPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class PutLaunchProfileMembersRequestRequestTypeDef(
     _RequiredPutLaunchProfileMembersRequestRequestTypeDef,
     _OptionalPutLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutStudioMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "members": Sequence[NewStudioMemberTypeDef],
         "studioId": str,
     },
@@ -1963,21 +1848,19 @@
     "_OptionalPutStudioMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
-
 class PutStudioMembersRequestRequestTypeDef(
     _RequiredPutStudioMembersRequestRequestTypeDef, _OptionalPutStudioMembersRequestRequestTypeDef
 ):
     pass
 
-
 StreamingSessionTypeDef = TypedDict(
     "StreamingSessionTypeDef",
     {
         "arn": str,
         "automaticTerminationMode": AutomaticTerminationModeType,
         "backupMode": SessionBackupModeType,
         "createdAt": datetime,
@@ -2004,58 +1887,34 @@
         "updatedBy": str,
         "volumeConfiguration": VolumeConfigurationTypeDef,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
-_RequiredStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
-    "_RequiredStreamConfigurationSessionStorageOutputTypeDef",
-    {
-        "mode": List[Literal["UPLOAD"]],
-    },
-)
-_OptionalStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
-    "_OptionalStreamConfigurationSessionStorageOutputTypeDef",
-    {
-        "root": StreamingSessionStorageRootTypeDef,
-    },
-    total=False,
-)
-
-
-class StreamConfigurationSessionStorageOutputTypeDef(
-    _RequiredStreamConfigurationSessionStorageOutputTypeDef,
-    _OptionalStreamConfigurationSessionStorageOutputTypeDef,
-):
-    pass
-
-
 _RequiredStreamConfigurationSessionStorageTypeDef = TypedDict(
     "_RequiredStreamConfigurationSessionStorageTypeDef",
     {
         "mode": Sequence[Literal["UPLOAD"]],
     },
 )
 _OptionalStreamConfigurationSessionStorageTypeDef = TypedDict(
     "_OptionalStreamConfigurationSessionStorageTypeDef",
     {
         "root": StreamingSessionStorageRootTypeDef,
     },
     total=False,
 )
 
-
 class StreamConfigurationSessionStorageTypeDef(
     _RequiredStreamConfigurationSessionStorageTypeDef,
     _OptionalStreamConfigurationSessionStorageTypeDef,
 ):
     pass
 
-
 StreamingImageTypeDef = TypedDict(
     "StreamingImageTypeDef",
     {
         "arn": str,
         "description": str,
         "ec2ImageId": str,
         "encryptionConfiguration": StreamingImageEncryptionConfigurationTypeDef,
@@ -2068,25 +1927,14 @@
         "statusMessage": str,
         "streamingImageId": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-StudioComponentConfigurationOutputTypeDef = TypedDict(
-    "StudioComponentConfigurationOutputTypeDef",
-    {
-        "activeDirectoryConfiguration": ActiveDirectoryConfigurationOutputTypeDef,
-        "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
-        "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
-        "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
-    },
-    total=False,
-)
-
 StudioComponentConfigurationTypeDef = TypedDict(
     "StudioComponentConfigurationTypeDef",
     {
         "activeDirectoryConfiguration": ActiveDirectoryConfigurationTypeDef,
         "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
         "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
         "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
@@ -2204,72 +2052,68 @@
     "StopStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStreamConfigurationTypeDef = TypedDict(
-    "_RequiredStreamConfigurationTypeDef",
+_RequiredStreamConfigurationCreateTypeDef = TypedDict(
+    "_RequiredStreamConfigurationCreateTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": List[StreamingInstanceTypeType],
-        "streamingImageIds": List[str],
+        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
+        "streamingImageIds": Sequence[str],
     },
 )
-_OptionalStreamConfigurationTypeDef = TypedDict(
-    "_OptionalStreamConfigurationTypeDef",
+_OptionalStreamConfigurationCreateTypeDef = TypedDict(
+    "_OptionalStreamConfigurationCreateTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
-        "sessionStorage": StreamConfigurationSessionStorageOutputTypeDef,
+        "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class StreamConfigurationTypeDef(
-    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
+class StreamConfigurationCreateTypeDef(
+    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
 ):
     pass
 
-
-_RequiredStreamConfigurationCreateTypeDef = TypedDict(
-    "_RequiredStreamConfigurationCreateTypeDef",
+_RequiredStreamConfigurationTypeDef = TypedDict(
+    "_RequiredStreamConfigurationTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
-        "streamingImageIds": Sequence[str],
+        "ec2InstanceTypes": List[StreamingInstanceTypeType],
+        "streamingImageIds": List[str],
     },
 )
-_OptionalStreamConfigurationCreateTypeDef = TypedDict(
-    "_OptionalStreamConfigurationCreateTypeDef",
+_OptionalStreamConfigurationTypeDef = TypedDict(
+    "_OptionalStreamConfigurationTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class StreamConfigurationCreateTypeDef(
-    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
+class StreamConfigurationTypeDef(
+    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
-
 CreateStreamingImageResponseTypeDef = TypedDict(
     "CreateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2303,41 +2147,14 @@
     "UpdateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StudioComponentTypeDef = TypedDict(
-    "StudioComponentTypeDef",
-    {
-        "arn": str,
-        "configuration": StudioComponentConfigurationOutputTypeDef,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SecurityGroupIds": List[str],
-        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
-        "name": str,
-        "runtimeRoleArn": str,
-        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
-        "secureInitializationRoleArn": str,
-        "state": StudioComponentStateType,
-        "statusCode": StudioComponentStatusCodeType,
-        "statusMessage": str,
-        "studioComponentId": str,
-        "subtype": StudioComponentSubtypeType,
-        "tags": Dict[str, str],
-        "type": StudioComponentTypeType,
-        "updatedAt": datetime,
-        "updatedBy": str,
-    },
-    total=False,
-)
-
 _RequiredCreateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioComponentRequestRequestTypeDef",
     {
         "name": str,
         "studioId": str,
         "type": StudioComponentTypeType,
     },
@@ -2355,25 +2172,47 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+StudioComponentTypeDef = TypedDict(
+    "StudioComponentTypeDef",
+    {
+        "arn": str,
+        "configuration": StudioComponentConfigurationTypeDef,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SecurityGroupIds": List[str],
+        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
+        "name": str,
+        "runtimeRoleArn": str,
+        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
+        "secureInitializationRoleArn": str,
+        "state": StudioComponentStateType,
+        "statusCode": StudioComponentStatusCodeType,
+        "statusMessage": str,
+        "studioComponentId": str,
+        "subtype": StudioComponentSubtypeType,
+        "tags": Dict[str, str],
+        "type": StudioComponentTypeType,
+        "updatedAt": datetime,
+        "updatedBy": str,
+    },
+    total=False,
+)
 
-StudioComponentConfigurationUnionTypeDef = Union[
-    StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
-]
 _RequiredUpdateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -2391,54 +2230,28 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "type": StudioComponentTypeType,
     },
     total=False,
 )
 
-
 class UpdateStudioComponentRequestRequestTypeDef(
     _RequiredUpdateStudioComponentRequestRequestTypeDef,
     _OptionalUpdateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-
 GetLaunchProfileInitializationResponseTypeDef = TypedDict(
     "GetLaunchProfileInitializationResponseTypeDef",
     {
         "launchProfileInitialization": LaunchProfileInitializationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LaunchProfileTypeDef = TypedDict(
-    "LaunchProfileTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SubnetIds": List[str],
-        "launchProfileId": str,
-        "launchProfileProtocolVersions": List[str],
-        "name": str,
-        "state": LaunchProfileStateType,
-        "statusCode": LaunchProfileStatusCodeType,
-        "statusMessage": str,
-        "streamConfiguration": StreamConfigurationTypeDef,
-        "studioComponentIds": List[str],
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "updatedBy": str,
-        "validationResults": List[ValidationResultTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchProfileRequestRequestTypeDef",
     {
         "ec2SubnetIds": Sequence[str],
         "launchProfileProtocolVersions": Sequence[str],
         "name": str,
         "streamConfiguration": StreamConfigurationCreateTypeDef,
@@ -2452,22 +2265,20 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateLaunchProfileRequestRequestTypeDef(
     _RequiredCreateLaunchProfileRequestRequestTypeDef,
     _OptionalCreateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -2480,21 +2291,43 @@
         "name": str,
         "streamConfiguration": StreamConfigurationCreateTypeDef,
         "studioComponentIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateLaunchProfileRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+LaunchProfileTypeDef = TypedDict(
+    "LaunchProfileTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SubnetIds": List[str],
+        "launchProfileId": str,
+        "launchProfileProtocolVersions": List[str],
+        "name": str,
+        "state": LaunchProfileStateType,
+        "statusCode": LaunchProfileStatusCodeType,
+        "statusMessage": str,
+        "streamConfiguration": StreamConfigurationTypeDef,
+        "studioComponentIds": List[str],
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "updatedBy": str,
+        "validationResults": List[ValidationResultTypeDef],
+    },
+    total=False,
+)
 
 CreateStudioComponentResponseTypeDef = TypedDict(
     "CreateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/type_defs.pyi` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_nimble.type_defs import AcceptEulasRequestRequestTypeDef
 
     data: AcceptEulasRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AutomaticTerminationModeType,
     LaunchProfilePlatformType,
     LaunchProfileStateType,
     LaunchProfileStatusCodeType,
     LaunchProfileValidationStateType,
@@ -49,14 +49,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptEulasRequestRequestTypeDef",
     "EulaAcceptanceTypeDef",
     "ResponseMetadataTypeDef",
     "ActiveDirectoryComputerAttributeTypeDef",
     "ComputeFarmConfigurationTypeDef",
     "CreateStreamingImageRequestRequestTypeDef",
@@ -120,15 +121,14 @@
     "UntagResourceRequestRequestTypeDef",
     "UpdateLaunchProfileMemberRequestRequestTypeDef",
     "UpdateStreamingImageRequestRequestTypeDef",
     "UpdateStudioRequestRequestTypeDef",
     "AcceptEulasResponseTypeDef",
     "ListEulaAcceptancesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ActiveDirectoryConfigurationOutputTypeDef",
     "ActiveDirectoryConfigurationTypeDef",
     "LaunchProfileInitializationActiveDirectoryTypeDef",
     "CreateStreamingSessionStreamResponseTypeDef",
     "GetStreamingSessionStreamResponseTypeDef",
     "CreateStudioRequestRequestTypeDef",
     "StudioTypeDef",
     "GetEulaResponseTypeDef",
@@ -161,47 +161,44 @@
     "ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     "ListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     "ListStudioMembersRequestListStudioMembersPaginateTypeDef",
     "ListStudiosRequestListStudiosPaginateTypeDef",
     "PutLaunchProfileMembersRequestRequestTypeDef",
     "PutStudioMembersRequestRequestTypeDef",
     "StreamingSessionTypeDef",
-    "StreamConfigurationSessionStorageOutputTypeDef",
     "StreamConfigurationSessionStorageTypeDef",
     "StreamingImageTypeDef",
-    "StudioComponentConfigurationOutputTypeDef",
     "StudioComponentConfigurationTypeDef",
     "LaunchProfileInitializationTypeDef",
     "CreateStudioResponseTypeDef",
     "DeleteStudioResponseTypeDef",
     "GetStudioResponseTypeDef",
     "ListStudiosResponseTypeDef",
     "StartStudioSSOConfigurationRepairResponseTypeDef",
     "UpdateStudioResponseTypeDef",
     "CreateStreamingSessionResponseTypeDef",
     "DeleteStreamingSessionResponseTypeDef",
     "GetStreamingSessionResponseTypeDef",
     "ListStreamingSessionsResponseTypeDef",
     "StartStreamingSessionResponseTypeDef",
     "StopStreamingSessionResponseTypeDef",
-    "StreamConfigurationTypeDef",
     "StreamConfigurationCreateTypeDef",
+    "StreamConfigurationTypeDef",
     "CreateStreamingImageResponseTypeDef",
     "DeleteStreamingImageResponseTypeDef",
     "GetStreamingImageResponseTypeDef",
     "ListStreamingImagesResponseTypeDef",
     "UpdateStreamingImageResponseTypeDef",
-    "StudioComponentTypeDef",
     "CreateStudioComponentRequestRequestTypeDef",
-    "StudioComponentConfigurationUnionTypeDef",
+    "StudioComponentTypeDef",
     "UpdateStudioComponentRequestRequestTypeDef",
     "GetLaunchProfileInitializationResponseTypeDef",
-    "LaunchProfileTypeDef",
     "CreateLaunchProfileRequestRequestTypeDef",
     "UpdateLaunchProfileRequestRequestTypeDef",
+    "LaunchProfileTypeDef",
     "CreateStudioComponentResponseTypeDef",
     "DeleteStudioComponentResponseTypeDef",
     "GetStudioComponentResponseTypeDef",
     "ListStudioComponentsResponseTypeDef",
     "UpdateStudioComponentResponseTypeDef",
     "CreateLaunchProfileResponseTypeDef",
     "DeleteLaunchProfileResponseTypeDef",
@@ -222,19 +219,21 @@
     {
         "clientToken": str,
         "eulaIds": Sequence[str],
     },
     total=False,
 )
 
+
 class AcceptEulasRequestRequestTypeDef(
     _RequiredAcceptEulasRequestRequestTypeDef, _OptionalAcceptEulasRequestRequestTypeDef
 ):
     pass
 
+
 EulaAcceptanceTypeDef = TypedDict(
     "EulaAcceptanceTypeDef",
     {
         "acceptedAt": datetime,
         "acceptedBy": str,
         "accepteeId": str,
         "eulaAcceptanceId": str,
@@ -286,20 +285,22 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStreamingImageRequestRequestTypeDef(
     _RequiredCreateStreamingImageRequestRequestTypeDef,
     _OptionalCreateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -311,20 +312,22 @@
         "ownedBy": str,
         "streamingImageId": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStreamingSessionRequestRequestTypeDef(
     _RequiredCreateStreamingSessionRequestRequestTypeDef,
     _OptionalCreateStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateStreamingSessionStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamingSessionStreamRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -333,20 +336,22 @@
     {
         "clientToken": str,
         "expirationInSeconds": int,
     },
     total=False,
 )
 
+
 class CreateStreamingSessionStreamRequestRequestTypeDef(
     _RequiredCreateStreamingSessionStreamRequestRequestTypeDef,
     _OptionalCreateStreamingSessionStreamRequestRequestTypeDef,
 ):
     pass
 
+
 StreamingSessionStreamTypeDef = TypedDict(
     "StreamingSessionStreamTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "expiresAt": datetime,
         "ownedBy": str,
@@ -388,19 +393,21 @@
     "_OptionalStudioEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
+
 class StudioEncryptionConfigurationTypeDef(
     _RequiredStudioEncryptionConfigurationTypeDef, _OptionalStudioEncryptionConfigurationTypeDef
 ):
     pass
 
+
 _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "principalId": str,
         "studioId": str,
     },
@@ -409,20 +416,22 @@
     "_OptionalDeleteLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteLaunchProfileMemberRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileMemberRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -430,20 +439,22 @@
     "_OptionalDeleteLaunchProfileRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteLaunchProfileRequestRequestTypeDef(
     _RequiredDeleteLaunchProfileRequestRequestTypeDef,
     _OptionalDeleteLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -451,20 +462,22 @@
     "_OptionalDeleteStreamingImageRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStreamingImageRequestRequestTypeDef(
     _RequiredDeleteStreamingImageRequestRequestTypeDef,
     _OptionalDeleteStreamingImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -472,20 +485,22 @@
     "_OptionalDeleteStreamingSessionRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStreamingSessionRequestRequestTypeDef(
     _RequiredDeleteStreamingSessionRequestRequestTypeDef,
     _OptionalDeleteStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -493,20 +508,22 @@
     "_OptionalDeleteStudioComponentRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStudioComponentRequestRequestTypeDef(
     _RequiredDeleteStudioComponentRequestRequestTypeDef,
     _OptionalDeleteStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStudioMemberRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioMemberRequestRequestTypeDef",
     {
         "principalId": str,
         "studioId": str,
     },
 )
@@ -514,39 +531,43 @@
     "_OptionalDeleteStudioMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStudioMemberRequestRequestTypeDef(
     _RequiredDeleteStudioMemberRequestRequestTypeDef,
     _OptionalDeleteStudioMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteStudioRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalDeleteStudioRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteStudioRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class DeleteStudioRequestRequestTypeDef(
     _RequiredDeleteStudioRequestRequestTypeDef, _OptionalDeleteStudioRequestRequestTypeDef
 ):
     pass
 
+
 EulaTypeDef = TypedDict(
     "EulaTypeDef",
     {
         "content": str,
         "createdAt": datetime,
         "eulaId": str,
         "name": str,
@@ -769,20 +790,22 @@
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListEulaAcceptancesRequestRequestTypeDef(
     _RequiredListEulaAcceptancesRequestRequestTypeDef,
     _OptionalListEulaAcceptancesRequestRequestTypeDef,
 ):
     pass
 
+
 ListEulasRequestRequestTypeDef = TypedDict(
     "ListEulasRequestRequestTypeDef",
     {
         "eulaIds": Sequence[str],
         "nextToken": str,
     },
     total=False,
@@ -800,20 +823,22 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListLaunchProfileMembersRequestRequestTypeDef(
     _RequiredListLaunchProfileMembersRequestRequestTypeDef,
     _OptionalListLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLaunchProfilesRequestRequestTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestRequestTypeDef = TypedDict(
@@ -823,20 +848,22 @@
         "nextToken": str,
         "principalId": str,
         "states": Sequence[LaunchProfileStateType],
     },
     total=False,
 )
 
+
 class ListLaunchProfilesRequestRequestTypeDef(
     _RequiredListLaunchProfilesRequestRequestTypeDef,
     _OptionalListLaunchProfilesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListStreamingImagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestRequestTypeDef = TypedDict(
@@ -844,20 +871,22 @@
     {
         "nextToken": str,
         "owner": str,
     },
     total=False,
 )
 
+
 class ListStreamingImagesRequestRequestTypeDef(
     _RequiredListStreamingImagesRequestRequestTypeDef,
     _OptionalListStreamingImagesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestRequestTypeDef = TypedDict(
@@ -865,20 +894,22 @@
     {
         "nextToken": str,
         "ownedBy": str,
     },
     total=False,
 )
 
+
 class ListStreamingSessionBackupsRequestRequestTypeDef(
     _RequiredListStreamingSessionBackupsRequestRequestTypeDef,
     _OptionalListStreamingSessionBackupsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListStreamingSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestRequestTypeDef = TypedDict(
@@ -888,20 +919,22 @@
         "nextToken": str,
         "ownedBy": str,
         "sessionIds": str,
     },
     total=False,
 )
 
+
 class ListStreamingSessionsRequestRequestTypeDef(
     _RequiredListStreamingSessionsRequestRequestTypeDef,
     _OptionalListStreamingSessionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListStudioComponentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestRequestTypeDef = TypedDict(
@@ -911,20 +944,22 @@
         "nextToken": str,
         "states": Sequence[StudioComponentStateType],
         "types": Sequence[StudioComponentTypeType],
     },
     total=False,
 )
 
+
 class ListStudioComponentsRequestRequestTypeDef(
     _RequiredListStudioComponentsRequestRequestTypeDef,
     _OptionalListStudioComponentsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestRequestTypeDef = TypedDict(
@@ -932,19 +967,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListStudioMembersRequestRequestTypeDef(
     _RequiredListStudioMembersRequestRequestTypeDef, _OptionalListStudioMembersRequestRequestTypeDef
 ):
     pass
 
+
 ListStudiosRequestRequestTypeDef = TypedDict(
     "ListStudiosRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -996,40 +1033,44 @@
     {
         "backupId": str,
         "clientToken": str,
     },
     total=False,
 )
 
+
 class StartStreamingSessionRequestRequestTypeDef(
     _RequiredStartStreamingSessionRequestRequestTypeDef,
     _OptionalStartStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef = TypedDict(
     "_OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class StartStudioSSOConfigurationRepairRequestRequestTypeDef(
     _RequiredStartStudioSSOConfigurationRepairRequestRequestTypeDef,
     _OptionalStartStudioSSOConfigurationRepairRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredStopStreamingSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStopStreamingSessionRequestRequestTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1038,20 +1079,22 @@
     {
         "clientToken": str,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
+
 class StopStreamingSessionRequestRequestTypeDef(
     _RequiredStopStreamingSessionRequestRequestTypeDef,
     _OptionalStopStreamingSessionRequestRequestTypeDef,
 ):
     pass
 
+
 StreamConfigurationSessionBackupTypeDef = TypedDict(
     "StreamConfigurationSessionBackupTypeDef",
     {
         "maxBackupsToRetain": int,
         "mode": SessionBackupModeType,
     },
     total=False,
@@ -1086,39 +1129,43 @@
     "_OptionalStreamingImageEncryptionConfigurationTypeDef",
     {
         "keyArn": str,
     },
     total=False,
 )
 
+
 class StreamingImageEncryptionConfigurationTypeDef(
     _RequiredStreamingImageEncryptionConfigurationTypeDef,
     _OptionalStreamingImageEncryptionConfigurationTypeDef,
 ):
     pass
 
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -1136,20 +1183,22 @@
     "_OptionalUpdateLaunchProfileMemberRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class UpdateLaunchProfileMemberRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileMemberRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileMemberRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateStreamingImageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamingImageRequestRequestTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1159,20 +1208,22 @@
         "clientToken": str,
         "description": str,
         "name": str,
     },
     total=False,
 )
 
+
 class UpdateStreamingImageRequestRequestTypeDef(
     _RequiredUpdateStreamingImageRequestRequestTypeDef,
     _OptionalUpdateStreamingImageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateStudioRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioRequestRequestTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalUpdateStudioRequestRequestTypeDef = TypedDict(
@@ -1182,19 +1233,21 @@
         "clientToken": str,
         "displayName": str,
         "userRoleArn": str,
     },
     total=False,
 )
 
+
 class UpdateStudioRequestRequestTypeDef(
     _RequiredUpdateStudioRequestRequestTypeDef, _OptionalUpdateStudioRequestRequestTypeDef
 ):
     pass
 
+
 AcceptEulasResponseTypeDef = TypedDict(
     "AcceptEulasResponseTypeDef",
     {
         "eulaAcceptances": List[EulaAcceptanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1212,24 +1265,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActiveDirectoryConfigurationOutputTypeDef = TypedDict(
-    "ActiveDirectoryConfigurationOutputTypeDef",
-    {
-        "computerAttributes": List[ActiveDirectoryComputerAttributeTypeDef],
-        "directoryId": str,
-        "organizationalUnitDistinguishedName": str,
-    },
-    total=False,
-)
-
 ActiveDirectoryConfigurationTypeDef = TypedDict(
     "ActiveDirectoryConfigurationTypeDef",
     {
         "computerAttributes": Sequence[ActiveDirectoryComputerAttributeTypeDef],
         "directoryId": str,
         "organizationalUnitDistinguishedName": str,
     },
@@ -1281,19 +1324,21 @@
         "clientToken": str,
         "studioEncryptionConfiguration": StudioEncryptionConfigurationTypeDef,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStudioRequestRequestTypeDef(
     _RequiredCreateStudioRequestRequestTypeDef, _OptionalCreateStudioRequestRequestTypeDef
 ):
     pass
 
+
 StudioTypeDef = TypedDict(
     "StudioTypeDef",
     {
         "adminRoleArn": str,
         "arn": str,
         "createdAt": datetime,
         "displayName": str,
@@ -1366,20 +1411,22 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef = TypedDict(
     "_RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -1387,20 +1434,22 @@
     "_OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetLaunchProfileRequestLaunchProfileReadyWaitTypeDef(
     _RequiredGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
     _OptionalGetLaunchProfileRequestLaunchProfileReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1408,20 +1457,22 @@
     "_OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingImageRequestStreamingImageDeletedWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "streamingImageId": str,
         "studioId": str,
     },
 )
@@ -1429,20 +1480,22 @@
     "_OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingImageRequestStreamingImageReadyWaitTypeDef(
     _RequiredGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
     _OptionalGetStreamingImageRequestStreamingImageReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1450,20 +1503,22 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1471,20 +1526,22 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionRequestStreamingSessionReadyWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "sessionId": str,
         "studioId": str,
     },
 )
@@ -1492,20 +1549,22 @@
     "_OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef(
     _RequiredGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
     _OptionalGetStreamingSessionRequestStreamingSessionStoppedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef = TypedDict(
     "_RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "sessionId": str,
         "streamId": str,
         "studioId": str,
     },
@@ -1514,20 +1573,22 @@
     "_OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef(
     _RequiredGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
     _OptionalGetStreamingSessionStreamRequestStreamingSessionStreamReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1535,20 +1596,22 @@
     "_OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioComponentRequestStudioComponentDeletedWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -1556,59 +1619,65 @@
     "_OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioComponentRequestStudioComponentReadyWaitTypeDef(
     _RequiredGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
     _OptionalGetStudioComponentRequestStudioComponentReadyWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioDeletedWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioDeletedWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioRequestStudioDeletedWaitTypeDef(
     _RequiredGetStudioRequestStudioDeletedWaitTypeDef,
     _OptionalGetStudioRequestStudioDeletedWaitTypeDef,
 ):
     pass
 
+
 _RequiredGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_RequiredGetStudioRequestStudioReadyWaitTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalGetStudioRequestStudioReadyWaitTypeDef = TypedDict(
     "_OptionalGetStudioRequestStudioReadyWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetStudioRequestStudioReadyWaitTypeDef(
     _RequiredGetStudioRequestStudioReadyWaitTypeDef, _OptionalGetStudioRequestStudioReadyWaitTypeDef
 ):
     pass
 
+
 GetStreamingSessionBackupResponseTypeDef = TypedDict(
     "GetStreamingSessionBackupResponseTypeDef",
     {
         "streamingSessionBackup": StreamingSessionBackupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1650,20 +1719,22 @@
     {
         "eulaIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef(
     _RequiredListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
     _OptionalListEulaAcceptancesRequestListEulaAcceptancesPaginateTypeDef,
 ):
     pass
 
+
 ListEulasRequestListEulasPaginateTypeDef = TypedDict(
     "ListEulasRequestListEulasPaginateTypeDef",
     {
         "eulaIds": Sequence[str],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1680,20 +1751,22 @@
     "_OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef(
     _RequiredListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
     _OptionalListLaunchProfileMembersRequestListLaunchProfileMembersPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
     "_RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef = TypedDict(
@@ -1702,20 +1775,22 @@
         "principalId": str,
         "states": Sequence[LaunchProfileStateType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef(
     _RequiredListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
     _OptionalListLaunchProfilesRequestListLaunchProfilesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
     "_RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef = TypedDict(
@@ -1723,20 +1798,22 @@
     {
         "owner": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStreamingImagesRequestListStreamingImagesPaginateTypeDef(
     _RequiredListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
     _OptionalListStreamingImagesRequestListStreamingImagesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
     "_RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef = TypedDict(
@@ -1744,20 +1821,22 @@
     {
         "ownedBy": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef(
     _RequiredListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
     _OptionalListStreamingSessionBackupsRequestListStreamingSessionBackupsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
     "_RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef = TypedDict(
@@ -1767,20 +1846,22 @@
         "ownedBy": str,
         "sessionIds": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef(
     _RequiredListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
     _OptionalListStreamingSessionsRequestListStreamingSessionsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
     "_RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef = TypedDict(
@@ -1789,40 +1870,44 @@
         "states": Sequence[StudioComponentStateType],
         "types": Sequence[StudioComponentTypeType],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStudioComponentsRequestListStudioComponentsPaginateTypeDef(
     _RequiredListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
     _OptionalListStudioComponentsRequestListStudioComponentsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
     "_RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef",
     {
         "studioId": str,
     },
 )
 _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef = TypedDict(
     "_OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListStudioMembersRequestListStudioMembersPaginateTypeDef(
     _RequiredListStudioMembersRequestListStudioMembersPaginateTypeDef,
     _OptionalListStudioMembersRequestListStudioMembersPaginateTypeDef,
 ):
     pass
 
+
 ListStudiosRequestListStudiosPaginateTypeDef = TypedDict(
     "ListStudiosRequestListStudiosPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1840,20 +1925,22 @@
     "_OptionalPutLaunchProfileMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class PutLaunchProfileMembersRequestRequestTypeDef(
     _RequiredPutLaunchProfileMembersRequestRequestTypeDef,
     _OptionalPutLaunchProfileMembersRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutStudioMembersRequestRequestTypeDef = TypedDict(
     "_RequiredPutStudioMembersRequestRequestTypeDef",
     {
         "identityStoreId": str,
         "members": Sequence[NewStudioMemberTypeDef],
         "studioId": str,
     },
@@ -1862,19 +1949,21 @@
     "_OptionalPutStudioMembersRequestRequestTypeDef",
     {
         "clientToken": str,
     },
     total=False,
 )
 
+
 class PutStudioMembersRequestRequestTypeDef(
     _RequiredPutStudioMembersRequestRequestTypeDef, _OptionalPutStudioMembersRequestRequestTypeDef
 ):
     pass
 
+
 StreamingSessionTypeDef = TypedDict(
     "StreamingSessionTypeDef",
     {
         "arn": str,
         "automaticTerminationMode": AutomaticTerminationModeType,
         "backupMode": SessionBackupModeType,
         "createdAt": datetime,
@@ -1901,54 +1990,36 @@
         "updatedBy": str,
         "volumeConfiguration": VolumeConfigurationTypeDef,
         "volumeRetentionMode": VolumeRetentionModeType,
     },
     total=False,
 )
 
-_RequiredStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
-    "_RequiredStreamConfigurationSessionStorageOutputTypeDef",
-    {
-        "mode": List[Literal["UPLOAD"]],
-    },
-)
-_OptionalStreamConfigurationSessionStorageOutputTypeDef = TypedDict(
-    "_OptionalStreamConfigurationSessionStorageOutputTypeDef",
-    {
-        "root": StreamingSessionStorageRootTypeDef,
-    },
-    total=False,
-)
-
-class StreamConfigurationSessionStorageOutputTypeDef(
-    _RequiredStreamConfigurationSessionStorageOutputTypeDef,
-    _OptionalStreamConfigurationSessionStorageOutputTypeDef,
-):
-    pass
-
 _RequiredStreamConfigurationSessionStorageTypeDef = TypedDict(
     "_RequiredStreamConfigurationSessionStorageTypeDef",
     {
         "mode": Sequence[Literal["UPLOAD"]],
     },
 )
 _OptionalStreamConfigurationSessionStorageTypeDef = TypedDict(
     "_OptionalStreamConfigurationSessionStorageTypeDef",
     {
         "root": StreamingSessionStorageRootTypeDef,
     },
     total=False,
 )
 
+
 class StreamConfigurationSessionStorageTypeDef(
     _RequiredStreamConfigurationSessionStorageTypeDef,
     _OptionalStreamConfigurationSessionStorageTypeDef,
 ):
     pass
 
+
 StreamingImageTypeDef = TypedDict(
     "StreamingImageTypeDef",
     {
         "arn": str,
         "description": str,
         "ec2ImageId": str,
         "encryptionConfiguration": StreamingImageEncryptionConfigurationTypeDef,
@@ -1961,25 +2032,14 @@
         "statusMessage": str,
         "streamingImageId": str,
         "tags": Dict[str, str],
     },
     total=False,
 )
 
-StudioComponentConfigurationOutputTypeDef = TypedDict(
-    "StudioComponentConfigurationOutputTypeDef",
-    {
-        "activeDirectoryConfiguration": ActiveDirectoryConfigurationOutputTypeDef,
-        "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
-        "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
-        "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
-    },
-    total=False,
-)
-
 StudioComponentConfigurationTypeDef = TypedDict(
     "StudioComponentConfigurationTypeDef",
     {
         "activeDirectoryConfiguration": ActiveDirectoryConfigurationTypeDef,
         "computeFarmConfiguration": ComputeFarmConfigurationTypeDef,
         "licenseServiceConfiguration": LicenseServiceConfigurationTypeDef,
         "sharedFileSystemConfiguration": SharedFileSystemConfigurationTypeDef,
@@ -2097,68 +2157,72 @@
     "StopStreamingSessionResponseTypeDef",
     {
         "session": StreamingSessionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStreamConfigurationTypeDef = TypedDict(
-    "_RequiredStreamConfigurationTypeDef",
+_RequiredStreamConfigurationCreateTypeDef = TypedDict(
+    "_RequiredStreamConfigurationCreateTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": List[StreamingInstanceTypeType],
-        "streamingImageIds": List[str],
+        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
+        "streamingImageIds": Sequence[str],
     },
 )
-_OptionalStreamConfigurationTypeDef = TypedDict(
-    "_OptionalStreamConfigurationTypeDef",
+_OptionalStreamConfigurationCreateTypeDef = TypedDict(
+    "_OptionalStreamConfigurationCreateTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
-        "sessionStorage": StreamConfigurationSessionStorageOutputTypeDef,
+        "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-class StreamConfigurationTypeDef(
-    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
+
+class StreamConfigurationCreateTypeDef(
+    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
 ):
     pass
 
-_RequiredStreamConfigurationCreateTypeDef = TypedDict(
-    "_RequiredStreamConfigurationCreateTypeDef",
+
+_RequiredStreamConfigurationTypeDef = TypedDict(
+    "_RequiredStreamConfigurationTypeDef",
     {
         "clipboardMode": StreamingClipboardModeType,
-        "ec2InstanceTypes": Sequence[StreamingInstanceTypeType],
-        "streamingImageIds": Sequence[str],
+        "ec2InstanceTypes": List[StreamingInstanceTypeType],
+        "streamingImageIds": List[str],
     },
 )
-_OptionalStreamConfigurationCreateTypeDef = TypedDict(
-    "_OptionalStreamConfigurationCreateTypeDef",
+_OptionalStreamConfigurationTypeDef = TypedDict(
+    "_OptionalStreamConfigurationTypeDef",
     {
         "automaticTerminationMode": AutomaticTerminationModeType,
         "maxSessionLengthInMinutes": int,
         "maxStoppedSessionLengthInMinutes": int,
         "sessionBackup": StreamConfigurationSessionBackupTypeDef,
         "sessionPersistenceMode": SessionPersistenceModeType,
         "sessionStorage": StreamConfigurationSessionStorageTypeDef,
         "volumeConfiguration": VolumeConfigurationTypeDef,
     },
     total=False,
 )
 
-class StreamConfigurationCreateTypeDef(
-    _RequiredStreamConfigurationCreateTypeDef, _OptionalStreamConfigurationCreateTypeDef
+
+class StreamConfigurationTypeDef(
+    _RequiredStreamConfigurationTypeDef, _OptionalStreamConfigurationTypeDef
 ):
     pass
 
+
 CreateStreamingImageResponseTypeDef = TypedDict(
     "CreateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2192,41 +2256,14 @@
     "UpdateStreamingImageResponseTypeDef",
     {
         "streamingImage": StreamingImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StudioComponentTypeDef = TypedDict(
-    "StudioComponentTypeDef",
-    {
-        "arn": str,
-        "configuration": StudioComponentConfigurationOutputTypeDef,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SecurityGroupIds": List[str],
-        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
-        "name": str,
-        "runtimeRoleArn": str,
-        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
-        "secureInitializationRoleArn": str,
-        "state": StudioComponentStateType,
-        "statusCode": StudioComponentStatusCodeType,
-        "statusMessage": str,
-        "studioComponentId": str,
-        "subtype": StudioComponentSubtypeType,
-        "tags": Dict[str, str],
-        "type": StudioComponentTypeType,
-        "updatedAt": datetime,
-        "updatedBy": str,
-    },
-    total=False,
-)
-
 _RequiredCreateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStudioComponentRequestRequestTypeDef",
     {
         "name": str,
         "studioId": str,
         "type": StudioComponentTypeType,
     },
@@ -2244,23 +2281,49 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStudioComponentRequestRequestTypeDef(
     _RequiredCreateStudioComponentRequestRequestTypeDef,
     _OptionalCreateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
-StudioComponentConfigurationUnionTypeDef = Union[
-    StudioComponentConfigurationTypeDef, StudioComponentConfigurationOutputTypeDef
-]
+
+StudioComponentTypeDef = TypedDict(
+    "StudioComponentTypeDef",
+    {
+        "arn": str,
+        "configuration": StudioComponentConfigurationTypeDef,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SecurityGroupIds": List[str],
+        "initializationScripts": List[StudioComponentInitializationScriptTypeDef],
+        "name": str,
+        "runtimeRoleArn": str,
+        "scriptParameters": List[ScriptParameterKeyValueTypeDef],
+        "secureInitializationRoleArn": str,
+        "state": StudioComponentStateType,
+        "statusCode": StudioComponentStatusCodeType,
+        "statusMessage": str,
+        "studioComponentId": str,
+        "subtype": StudioComponentSubtypeType,
+        "tags": Dict[str, str],
+        "type": StudioComponentTypeType,
+        "updatedAt": datetime,
+        "updatedBy": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateStudioComponentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStudioComponentRequestRequestTypeDef",
     {
         "studioComponentId": str,
         "studioId": str,
     },
 )
@@ -2278,52 +2341,30 @@
         "secureInitializationRoleArn": str,
         "subtype": StudioComponentSubtypeType,
         "type": StudioComponentTypeType,
     },
     total=False,
 )
 
+
 class UpdateStudioComponentRequestRequestTypeDef(
     _RequiredUpdateStudioComponentRequestRequestTypeDef,
     _OptionalUpdateStudioComponentRequestRequestTypeDef,
 ):
     pass
 
+
 GetLaunchProfileInitializationResponseTypeDef = TypedDict(
     "GetLaunchProfileInitializationResponseTypeDef",
     {
         "launchProfileInitialization": LaunchProfileInitializationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LaunchProfileTypeDef = TypedDict(
-    "LaunchProfileTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "description": str,
-        "ec2SubnetIds": List[str],
-        "launchProfileId": str,
-        "launchProfileProtocolVersions": List[str],
-        "name": str,
-        "state": LaunchProfileStateType,
-        "statusCode": LaunchProfileStatusCodeType,
-        "statusMessage": str,
-        "streamConfiguration": StreamConfigurationTypeDef,
-        "studioComponentIds": List[str],
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "updatedBy": str,
-        "validationResults": List[ValidationResultTypeDef],
-    },
-    total=False,
-)
-
 _RequiredCreateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLaunchProfileRequestRequestTypeDef",
     {
         "ec2SubnetIds": Sequence[str],
         "launchProfileProtocolVersions": Sequence[str],
         "name": str,
         "streamConfiguration": StreamConfigurationCreateTypeDef,
@@ -2337,20 +2378,22 @@
         "clientToken": str,
         "description": str,
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateLaunchProfileRequestRequestTypeDef(
     _RequiredCreateLaunchProfileRequestRequestTypeDef,
     _OptionalCreateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateLaunchProfileRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLaunchProfileRequestRequestTypeDef",
     {
         "launchProfileId": str,
         "studioId": str,
     },
 )
@@ -2363,20 +2406,46 @@
         "name": str,
         "streamConfiguration": StreamConfigurationCreateTypeDef,
         "studioComponentIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateLaunchProfileRequestRequestTypeDef(
     _RequiredUpdateLaunchProfileRequestRequestTypeDef,
     _OptionalUpdateLaunchProfileRequestRequestTypeDef,
 ):
     pass
 
+
+LaunchProfileTypeDef = TypedDict(
+    "LaunchProfileTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "description": str,
+        "ec2SubnetIds": List[str],
+        "launchProfileId": str,
+        "launchProfileProtocolVersions": List[str],
+        "name": str,
+        "state": LaunchProfileStateType,
+        "statusCode": LaunchProfileStatusCodeType,
+        "statusMessage": str,
+        "streamConfiguration": StreamConfigurationTypeDef,
+        "studioComponentIds": List[str],
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "updatedBy": str,
+        "validationResults": List[ValidationResultTypeDef],
+    },
+    total=False,
+)
+
 CreateStudioComponentResponseTypeDef = TypedDict(
     "CreateStudioComponentResponseTypeDef",
     {
         "studioComponent": StudioComponentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.py` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble/waiter.pyi` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-nimble-2.5.2.post1/types_aiobotocore_nimble.egg-info/SOURCES.txt` & `types-aiobotocore-nimble-2.5.2.post2/types_aiobotocore_nimble.egg-info/SOURCES.txt`

 * *Files identical despite different names*

