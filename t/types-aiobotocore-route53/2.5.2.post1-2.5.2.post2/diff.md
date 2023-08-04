# Comparing `tmp/types-aiobotocore-route53-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-route53-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-route53-2.5.2.post1.tar` & `types-aiobotocore-route53-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58287 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63226 2023-08-02 14:48:05.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63155 2023-08-02 14:48:05.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.796643 types-aiobotocore-route53-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14843 2023-08-04 13:59:23.796643 types-aiobotocore-route53-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13325 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.796643 types-aiobotocore-route53-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2072 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.796643 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2557 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2556 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      943 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58365 2023-08-04 13:51:01.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    58277 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13172 2023-08-04 13:51:04.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13170 2023-08-04 13:51:04.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10219 2023-08-04 13:51:01.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10209 2023-08-04 13:51:01.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    61067 2023-08-04 13:51:05.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    61000 2023-08-04 13:51:05.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:00.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1626 2023-08-04 13:51:01.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1625 2023-08-04 13:51:01.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.796643 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14843 2023-08-04 13:59:23.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      886 2023-08-04 13:59:23.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       26 2023-08-04 13:59:23.000000 types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-2.5.2.post1/LICENSE` & `types-aiobotocore-route53-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/setup.py` & `types-aiobotocore-route53-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.pyi` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__main__.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Route53 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     GetHostedZoneResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyResponseTypeDef,
-    HealthCheckConfigUnionTypeDef,
+    HealthCheckConfigTypeDef,
     HostedZoneConfigTypeDef,
     ListCidrBlocksResponseTypeDef,
     ListCidrCollectionsResponseTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListGeoLocationsResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
@@ -303,15 +303,15 @@
         Creates a CIDR collection in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_cidr_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_cidr_collection)
         """
 
     async def create_health_check(
-        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigUnionTypeDef
+        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigTypeDef
     ) -> CreateHealthCheckResponseTypeDef:
         """
         Creates a new health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_health_check)
         """
```

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.pyi` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     GetHostedZoneResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyResponseTypeDef,
-    HealthCheckConfigUnionTypeDef,
+    HealthCheckConfigTypeDef,
     HostedZoneConfigTypeDef,
     ListCidrBlocksResponseTypeDef,
     ListCidrCollectionsResponseTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListGeoLocationsResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
@@ -290,15 +290,15 @@
         """
         Creates a CIDR collection in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_cidr_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_cidr_collection)
         """
     async def create_health_check(
-        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigUnionTypeDef
+        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigTypeDef
     ) -> CreateHealthCheckResponseTypeDef:
         """
         Creates a new health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_health_check)
         """
```

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
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
     "us-gov-east-1",
     "us-gov-west-1",
@@ -163,14 +164,15 @@
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
@@ -197,14 +199,15 @@
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
     "us-gov-east-1",
     "us-gov-west-1",
@@ -226,14 +229,15 @@
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
@@ -329,14 +333,15 @@
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
@@ -415,26 +420,28 @@
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

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.pyi` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
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
     "us-gov-east-1",
     "us-gov-west-1",
@@ -161,14 +162,15 @@
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
@@ -195,14 +197,15 @@
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
     "us-gov-east-1",
     "us-gov-west-1",
@@ -224,14 +227,15 @@
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
@@ -327,14 +331,15 @@
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
@@ -413,26 +418,28 @@
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

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.pyi` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_route53.type_defs import AccountLimitTypeDef
 
     data: AccountLimitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AccountLimitTypeType,
     ChangeActionType,
     ChangeStatusType,
     CidrCollectionChangeActionType,
     CloudWatchRegionType,
@@ -147,15 +147,14 @@
     "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
     "GetCheckerIpRangesResponseTypeDef",
     "GetHealthCheckCountResponseTypeDef",
     "GetHostedZoneCountResponseTypeDef",
     "GetTrafficPolicyInstanceCountResponseTypeDef",
     "TestDNSAnswerResponseTypeDef",
-    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
@@ -201,31 +200,29 @@
     "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
-    "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
-    "HealthCheckConfigUnionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
-    "ListResourceRecordSetsResponseTypeDef",
     "ChangeTypeDef",
+    "ListResourceRecordSetsResponseTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -1376,51 +1373,14 @@
         "RecordData": List[str],
         "ResponseCode": str,
         "Protocol": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckConfigOutputTypeDef",
-    {
-        "Type": HealthCheckTypeType,
-    },
-)
-_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckConfigOutputTypeDef",
-    {
-        "IPAddress": str,
-        "Port": int,
-        "ResourcePath": str,
-        "FullyQualifiedDomainName": str,
-        "SearchString": str,
-        "RequestInterval": int,
-        "FailureThreshold": int,
-        "MeasureLatency": bool,
-        "Inverted": bool,
-        "Disabled": bool,
-        "HealthThreshold": int,
-        "ChildHealthChecks": List[str],
-        "EnableSNI": bool,
-        "Regions": List[HealthCheckRegionType],
-        "AlarmIdentifier": AlarmIdentifierTypeDef,
-        "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
-        "RoutingControlArn": str,
-    },
-    total=False,
-)
-
-
-class HealthCheckConfigOutputTypeDef(
-    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
     },
 )
 _OptionalHealthCheckConfigTypeDef = TypedDict(
@@ -2131,47 +2091,14 @@
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredResourceRecordSetOutputTypeDef = TypedDict(
-    "_RequiredResourceRecordSetOutputTypeDef",
-    {
-        "Name": str,
-        "Type": RRTypeType,
-    },
-)
-_OptionalResourceRecordSetOutputTypeDef = TypedDict(
-    "_OptionalResourceRecordSetOutputTypeDef",
-    {
-        "SetIdentifier": str,
-        "Weight": int,
-        "Region": ResourceRecordSetRegionType,
-        "GeoLocation": GeoLocationTypeDef,
-        "Failover": ResourceRecordSetFailoverType,
-        "MultiValueAnswer": bool,
-        "TTL": int,
-        "ResourceRecords": List[ResourceRecordTypeDef],
-        "AliasTarget": AliasTargetTypeDef,
-        "HealthCheckId": str,
-        "TrafficPolicyInstanceId": str,
-        "CidrRoutingConfig": CidrRoutingConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class ResourceRecordSetOutputTypeDef(
-    _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
-):
-    pass
-
-
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
         "Type": RRTypeType,
     },
 )
@@ -2205,15 +2132,14 @@
     "CreateHealthCheckRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
-HealthCheckConfigUnionTypeDef = Union[HealthCheckConfigTypeDef, HealthCheckConfigOutputTypeDef]
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTagSet": ResourceTagSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2227,15 +2153,15 @@
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckVersion": int,
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "LinkedService": LinkedServiceTypeDef,
@@ -2327,35 +2253,35 @@
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ChangeTypeDef = TypedDict(
+    "ChangeTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ResourceRecordSet": ResourceRecordSetTypeDef,
+    },
+)
+
 ListResourceRecordSetsResponseTypeDef = TypedDict(
     "ListResourceRecordSetsResponseTypeDef",
     {
-        "ResourceRecordSets": List[ResourceRecordSetOutputTypeDef],
+        "ResourceRecordSets": List[ResourceRecordSetTypeDef],
         "IsTruncated": bool,
         "NextRecordName": str,
         "NextRecordType": RRTypeType,
         "NextRecordIdentifier": str,
         "MaxItems": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChangeTypeDef = TypedDict(
-    "ChangeTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ResourceRecordSet": ResourceRecordSetTypeDef,
-    },
-)
-
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.pyi` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_route53.type_defs import AccountLimitTypeDef
 
     data: AccountLimitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AccountLimitTypeType,
     ChangeActionType,
     ChangeStatusType,
     CidrCollectionChangeActionType,
     CloudWatchRegionType,
@@ -146,15 +146,14 @@
     "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
     "GetCheckerIpRangesResponseTypeDef",
     "GetHealthCheckCountResponseTypeDef",
     "GetHostedZoneCountResponseTypeDef",
     "GetTrafficPolicyInstanceCountResponseTypeDef",
     "TestDNSAnswerResponseTypeDef",
-    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
@@ -200,31 +199,29 @@
     "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
-    "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
-    "HealthCheckConfigUnionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
-    "ListResourceRecordSetsResponseTypeDef",
     "ChangeTypeDef",
+    "ListResourceRecordSetsResponseTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -1343,49 +1340,14 @@
         "RecordData": List[str],
         "ResponseCode": str,
         "Protocol": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckConfigOutputTypeDef",
-    {
-        "Type": HealthCheckTypeType,
-    },
-)
-_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckConfigOutputTypeDef",
-    {
-        "IPAddress": str,
-        "Port": int,
-        "ResourcePath": str,
-        "FullyQualifiedDomainName": str,
-        "SearchString": str,
-        "RequestInterval": int,
-        "FailureThreshold": int,
-        "MeasureLatency": bool,
-        "Inverted": bool,
-        "Disabled": bool,
-        "HealthThreshold": int,
-        "ChildHealthChecks": List[str],
-        "EnableSNI": bool,
-        "Regions": List[HealthCheckRegionType],
-        "AlarmIdentifier": AlarmIdentifierTypeDef,
-        "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
-        "RoutingControlArn": str,
-    },
-    total=False,
-)
-
-class HealthCheckConfigOutputTypeDef(
-    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
-):
-    pass
-
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
     },
 )
 _OptionalHealthCheckConfigTypeDef = TypedDict(
@@ -2068,45 +2030,14 @@
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredResourceRecordSetOutputTypeDef = TypedDict(
-    "_RequiredResourceRecordSetOutputTypeDef",
-    {
-        "Name": str,
-        "Type": RRTypeType,
-    },
-)
-_OptionalResourceRecordSetOutputTypeDef = TypedDict(
-    "_OptionalResourceRecordSetOutputTypeDef",
-    {
-        "SetIdentifier": str,
-        "Weight": int,
-        "Region": ResourceRecordSetRegionType,
-        "GeoLocation": GeoLocationTypeDef,
-        "Failover": ResourceRecordSetFailoverType,
-        "MultiValueAnswer": bool,
-        "TTL": int,
-        "ResourceRecords": List[ResourceRecordTypeDef],
-        "AliasTarget": AliasTargetTypeDef,
-        "HealthCheckId": str,
-        "TrafficPolicyInstanceId": str,
-        "CidrRoutingConfig": CidrRoutingConfigTypeDef,
-    },
-    total=False,
-)
-
-class ResourceRecordSetOutputTypeDef(
-    _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
-):
-    pass
-
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
         "Type": RRTypeType,
     },
 )
@@ -2138,15 +2069,14 @@
     "CreateHealthCheckRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
-HealthCheckConfigUnionTypeDef = Union[HealthCheckConfigTypeDef, HealthCheckConfigOutputTypeDef]
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTagSet": ResourceTagSetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2160,15 +2090,15 @@
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
+        "HealthCheckConfig": HealthCheckConfigTypeDef,
         "HealthCheckVersion": int,
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "LinkedService": LinkedServiceTypeDef,
@@ -2258,35 +2188,35 @@
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ChangeTypeDef = TypedDict(
+    "ChangeTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ResourceRecordSet": ResourceRecordSetTypeDef,
+    },
+)
+
 ListResourceRecordSetsResponseTypeDef = TypedDict(
     "ListResourceRecordSetsResponseTypeDef",
     {
-        "ResourceRecordSets": List[ResourceRecordSetOutputTypeDef],
+        "ResourceRecordSets": List[ResourceRecordSetTypeDef],
         "IsTruncated": bool,
         "NextRecordName": str,
         "NextRecordType": RRTypeType,
         "NextRecordIdentifier": str,
         "MaxItems": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChangeTypeDef = TypedDict(
-    "ChangeTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ResourceRecordSet": ResourceRecordSetTypeDef,
-    },
-)
-
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.py` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.pyi` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/SOURCES.txt` & `types-aiobotocore-route53-2.5.2.post2/types_aiobotocore_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

