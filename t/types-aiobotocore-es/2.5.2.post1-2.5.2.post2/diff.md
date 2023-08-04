# Comparing `tmp/types-aiobotocore-es-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-es-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-es-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-es-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:53 2023, max compression
```

## Comparing `types-aiobotocore-es-2.5.2.post1.tar` & `types-aiobotocore-es-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21213 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.965588 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43183 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43119 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64435 2023-08-02 14:38:35.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64388 2023-08-02 14:38:33.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:32.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:16.969588 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22729 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:16.000000 types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.040165 types-aiobotocore-es-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-08-04 12:00:53.040165 types-aiobotocore-es-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:53.040165 types-aiobotocore-es-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.032165 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43173 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43109 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-08-04 11:46:02.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7547 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63653 2023-08-04 11:46:04.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63606 2023-08-04 11:46:02.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:01.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.040165 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-08-04 12:00:52.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 12:00:52.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 12:00:52.000000 types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-es-2.5.2.post1/LICENSE` & `types-aiobotocore-es-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/setup.py` & `types-aiobotocore-es-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-es",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_es"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticsearchService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.py` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__init__.pyi` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/__main__.py` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticsearchService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_es//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService\nOther"
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

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.py` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from .type_defs import (
     AcceptInboundCrossClusterSearchConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsUnionTypeDef,
+    AutoTuneOptionsTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     CognitoOptionsTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
     CreateOutboundCrossClusterSearchConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteElasticsearchDomainResponseTypeDef,
@@ -707,15 +707,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...
     ) -> UpdateElasticsearchDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Elasticsearch domain,
         setting as setting the instance type and the number of instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_elasticsearch_domain_config)
```

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/client.pyi` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 )
 from .type_defs import (
     AcceptInboundCrossClusterSearchConnectionResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsUnionTypeDef,
+    AutoTuneOptionsTypeDef,
     CancelElasticsearchServiceSoftwareUpdateResponseTypeDef,
     CognitoOptionsTypeDef,
     CreateElasticsearchDomainResponseTypeDef,
     CreateOutboundCrossClusterSearchConnectionResponseTypeDef,
     CreatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DeleteElasticsearchDomainResponseTypeDef,
@@ -653,15 +653,15 @@
         AdvancedOptions: Mapping[str, str] = ...,
         AccessPolicies: str = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
         DryRun: bool = ...
     ) -> UpdateElasticsearchDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Elasticsearch domain,
         setting as setting the instance type and the number of instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Client.update_elasticsearch_domain_config)
```

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.py` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/literals.pyi` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.py` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/paginator.pyi` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.py` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,14 @@
     "AdvancedOptionsStatusTypeDef",
     "ElasticsearchVersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "UpgradeElasticsearchDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
@@ -193,15 +192,14 @@
     "ReservedElasticsearchInstanceOfferingTypeDef",
     "ReservedElasticsearchInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "AutoTuneTypeDef",
-    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
@@ -223,15 +221,14 @@
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
-    "AutoTuneOptionsUnionTypeDef",
     "CreateElasticsearchDomainRequestRequestTypeDef",
     "UpdateElasticsearchDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "ElasticsearchDomainStatusTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     "ElasticsearchDomainConfigTypeDef",
     "CreateElasticsearchDomainResponseTypeDef",
@@ -1269,24 +1266,14 @@
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
-    {
-        "StartAt": datetime,
-        "Duration": DurationTypeDef,
-        "CronExpressionForRecurrence": str,
-    },
-    total=False,
-)
-
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
@@ -1830,39 +1817,29 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsExtraOutputTypeDef = TypedDict(
-    "AutoTuneOptionsExtraOutputTypeDef",
-    {
-        "DesiredState": AutoTuneDesiredStateType,
-        "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
-    },
-    total=False,
-)
-
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
@@ -2092,21 +2069,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsExtraOutputTypeDef,
+        "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 _RequiredCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateElasticsearchDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es/type_defs.pyi` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,14 @@
     "AdvancedOptionsStatusTypeDef",
     "ElasticsearchVersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "CancelElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "StartElasticsearchServiceSoftwareUpdateResponseTypeDef",
     "UpgradeElasticsearchDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleElasticsearchVersionsResponseTypeDef",
@@ -192,15 +191,14 @@
     "ReservedElasticsearchInstanceOfferingTypeDef",
     "ReservedElasticsearchInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "AutoTuneTypeDef",
-    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "DeleteOutboundCrossClusterSearchConnectionResponseTypeDef",
     "DescribeOutboundCrossClusterSearchConnectionsResponseTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
@@ -222,15 +220,14 @@
     "DescribeReservedElasticsearchInstancesResponseTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
     "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
-    "AutoTuneOptionsUnionTypeDef",
     "CreateElasticsearchDomainRequestRequestTypeDef",
     "UpdateElasticsearchDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
     "ElasticsearchDomainStatusTypeDef",
     "DescribeElasticsearchInstanceTypeLimitsResponseTypeDef",
     "ElasticsearchDomainConfigTypeDef",
     "CreateElasticsearchDomainResponseTypeDef",
@@ -1238,24 +1235,14 @@
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": ScheduledAutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
-    "AutoTuneMaintenanceScheduleOutputTypeDef",
-    {
-        "StartAt": datetime,
-        "Duration": DurationTypeDef,
-        "CronExpressionForRecurrence": str,
-    },
-    total=False,
-)
-
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": TimestampTypeDef,
         "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
@@ -1789,39 +1776,29 @@
     {
         "AutoTuneType": Literal["SCHEDULED_ACTION"],
         "AutoTuneDetails": AutoTuneDetailsTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsExtraOutputTypeDef = TypedDict(
-    "AutoTuneOptionsExtraOutputTypeDef",
-    {
-        "DesiredState": AutoTuneDesiredStateType,
-        "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleOutputTypeDef],
-    },
-    total=False,
-)
-
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": AutoTuneDesiredStateType,
         "RollbackOnDisable": RollbackOnDisableType,
-        "MaintenanceSchedules": Sequence[AutoTuneMaintenanceScheduleTypeDef],
+        "MaintenanceSchedules": List[AutoTuneMaintenanceScheduleTypeDef],
     },
     total=False,
 )
 
 DescribeDomainChangeProgressResponseTypeDef = TypedDict(
     "DescribeDomainChangeProgressResponseTypeDef",
     {
@@ -2051,21 +2028,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": AutoTuneOptionsExtraOutputTypeDef,
+        "Options": AutoTuneOptionsTypeDef,
         "Status": AutoTuneStatusTypeDef,
     },
     total=False,
 )
 
-AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 _RequiredCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateElasticsearchDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateElasticsearchDomainRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-es-2.5.2.post1/types_aiobotocore_es.egg-info/SOURCES.txt` & `types-aiobotocore-es-2.5.2.post2/types_aiobotocore_es.egg-info/SOURCES.txt`

 * *Files identical despite different names*

