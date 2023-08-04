# Comparing `tmp/types-aiobotocore-customer-profiles-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-customer-profiles-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-customer-profiles-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:42 2023, max compression
```

## Comparing `types-aiobotocore-customer-profiles-2.5.2.post1.tar` & `types-aiobotocore-customer-profiles-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.561612 types-aiobotocore-customer-profiles-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-02 14:52:07.561612 types-aiobotocore-customer-profiles-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18714 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.561612 types-aiobotocore-customer-profiles-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.561612 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41047 2023-08-02 14:35:59.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40988 2023-08-02 14:35:59.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-08-02 14:35:59.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-08-02 14:35:59.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 14:35:59.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-02 14:35:59.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64592 2023-08-02 14:36:01.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64502 2023-08-02 14:36:00.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:58.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.561612 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20271 2023-08-02 14:52:07.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:07.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:07.000000 types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.207754 types-aiobotocore-customer-profiles-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:00:42.203754 types-aiobotocore-customer-profiles-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:42.207754 types-aiobotocore-customer-profiles-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.195753 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41017 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40958 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12679 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62983 2023-08-04 11:43:21.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62895 2023-08-04 11:43:19.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:18.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:42.203754 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13544 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:42.000000 types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/LICENSE` & `types-aiobotocore-customer-profiles-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/setup.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-customer-profiles",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CustomerProfiles 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/__init__.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/__init__.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/__main__.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CustomerProfiles 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
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

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/client.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
-    AttributeDetailsUnionTypeDef,
+    AttributeDetailsTypeDef,
     ConditionsTypeDef,
     ConflictResolutionTypeDef,
-    ConsolidationUnionTypeDef,
+    ConsolidationTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteIntegrationResponseTypeDef,
@@ -68,15 +68,15 @@
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
-    ObjectTypeKeyUnionTypeDef,
+    ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     SearchProfilesResponseTypeDef,
     TimestampTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
@@ -155,15 +155,15 @@
         """
 
     async def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
-        AttributeDetails: AttributeDetailsUnionTypeDef,
+        AttributeDetails: AttributeDetailsTypeDef,
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
@@ -354,15 +354,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#generate_presigned_url)
         """
 
     async def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
-        Consolidation: ConsolidationUnionTypeDef,
+        Consolidation: ConsolidationTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
@@ -674,15 +674,15 @@
         Description: str,
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
-        Keys: Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]] = ...,
+        Keys: Mapping[str, Sequence[ObjectTypeKeyTypeDef]] = ...,
         Tags: Mapping[str, str] = ...
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#put_profile_object_type)
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/client.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
 from .literals import GenderType, PartyTypeType, StatisticType, StatusType, logicalOperatorType
 from .paginator import ListEventStreamsPaginator
 from .type_defs import (
     AdditionalSearchKeyTypeDef,
     AddProfileKeyResponseTypeDef,
     AddressTypeDef,
-    AttributeDetailsUnionTypeDef,
+    AttributeDetailsTypeDef,
     ConditionsTypeDef,
     ConflictResolutionTypeDef,
-    ConsolidationUnionTypeDef,
+    ConsolidationTypeDef,
     CreateCalculatedAttributeDefinitionResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateEventStreamResponseTypeDef,
     CreateIntegrationWorkflowResponseTypeDef,
     CreateProfileResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DeleteIntegrationResponseTypeDef,
@@ -68,15 +68,15 @@
     ListProfileObjectTypeTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWorkflowsResponseTypeDef,
     MatchingRequestTypeDef,
     MergeProfilesResponseTypeDef,
     ObjectFilterTypeDef,
     ObjectTypeFieldTypeDef,
-    ObjectTypeKeyUnionTypeDef,
+    ObjectTypeKeyTypeDef,
     PutIntegrationResponseTypeDef,
     PutProfileObjectResponseTypeDef,
     PutProfileObjectTypeResponseTypeDef,
     SearchProfilesResponseTypeDef,
     TimestampTypeDef,
     UpdateAddressTypeDef,
     UpdateCalculatedAttributeDefinitionResponseTypeDef,
@@ -147,15 +147,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#close)
         """
     async def create_calculated_attribute_definition(
         self,
         *,
         DomainName: str,
         CalculatedAttributeName: str,
-        AttributeDetails: AttributeDetailsUnionTypeDef,
+        AttributeDetails: AttributeDetailsTypeDef,
         Statistic: StatisticType,
         DisplayName: str = ...,
         Description: str = ...,
         Conditions: ConditionsTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateCalculatedAttributeDefinitionResponseTypeDef:
         """
@@ -331,15 +331,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#generate_presigned_url)
         """
     async def get_auto_merging_preview(
         self,
         *,
         DomainName: str,
-        Consolidation: ConsolidationUnionTypeDef,
+        Consolidation: ConsolidationTypeDef,
         ConflictResolution: ConflictResolutionTypeDef,
         MinAllowedConfidenceScoreForMerging: float = ...
     ) -> GetAutoMergingPreviewResponseTypeDef:
         """
         Tests the auto-merging settings of your Identity Resolution Job without merging
         your data.
 
@@ -624,15 +624,15 @@
         Description: str,
         TemplateId: str = ...,
         ExpirationDays: int = ...,
         EncryptionKey: str = ...,
         AllowProfileCreation: bool = ...,
         SourceLastUpdatedTimestampFormat: str = ...,
         Fields: Mapping[str, ObjectTypeFieldTypeDef] = ...,
-        Keys: Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]] = ...,
+        Keys: Mapping[str, Sequence[ObjectTypeKeyTypeDef]] = ...,
         Tags: Mapping[str, str] = ...
     ) -> PutProfileObjectTypeResponseTypeDef:
         """
         Defines a ProfileObjectType.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.put_profile_object_type)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_customer_profiles/client/#put_profile_object_type)
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/literals.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/literals.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/paginator.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/paginator.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/type_defs.py` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
     "AttributeItemTypeDef",
     "ConflictResolutionTypeDef",
-    "ConsolidationOutputTypeDef",
     "ConsolidationTypeDef",
     "TimestampTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
@@ -91,15 +90,15 @@
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldTypeDef",
-    "ObjectTypeKeyOutputTypeDef",
+    "ObjectTypeKeyTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
@@ -118,15 +117,14 @@
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkflowsItemTypeDef",
     "MarketoSourcePropertiesTypeDef",
-    "ObjectTypeKeyTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -150,19 +148,16 @@
     "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
-    "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
-    "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
-    "ConsolidationUnionTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
     "BatchTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
@@ -170,45 +165,43 @@
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
+    "PutProfileObjectTypeRequestRequestTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "ObjectTypeKeyUnionTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
-    "AttributeDetailsUnionTypeDef",
     "TriggerPropertiesTypeDef",
     "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
-    "PutProfileObjectTypeRequestRequestTypeDef",
     "SourceFlowConfigTypeDef",
     "TriggerConfigTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
@@ -336,21 +329,14 @@
 
 class ConflictResolutionTypeDef(
     _RequiredConflictResolutionTypeDef, _OptionalConflictResolutionTypeDef
 ):
     pass
 
 
-ConsolidationOutputTypeDef = TypedDict(
-    "ConsolidationOutputTypeDef",
-    {
-        "MatchingAttributesList": List[List[str]],
-    },
-)
-
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
@@ -708,16 +694,16 @@
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
     total=False,
 )
 
-ObjectTypeKeyOutputTypeDef = TypedDict(
-    "ObjectTypeKeyOutputTypeDef",
+ObjectTypeKeyTypeDef = TypedDict(
+    "ObjectTypeKeyTypeDef",
     {
         "StandardIdentifiers": List[StandardIdentifierType],
         "FieldNames": List[str],
     },
     total=False,
 )
 
@@ -1112,23 +1098,14 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
-ObjectTypeKeyTypeDef = TypedDict(
-    "ObjectTypeKeyTypeDef",
-    {
-        "StandardIdentifiers": Sequence[StandardIdentifierType],
-        "FieldNames": Sequence[str],
-    },
-    total=False,
-)
-
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
@@ -1482,53 +1459,22 @@
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
     total=False,
 )
 
-AttributeDetailsOutputTypeDef = TypedDict(
-    "AttributeDetailsOutputTypeDef",
-    {
-        "Attributes": List[AttributeItemTypeDef],
-        "Expression": str,
-    },
-)
-
 AttributeDetailsTypeDef = TypedDict(
     "AttributeDetailsTypeDef",
     {
         "Attributes": Sequence[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
-_RequiredAutoMergingOutputTypeDef = TypedDict(
-    "_RequiredAutoMergingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalAutoMergingOutputTypeDef = TypedDict(
-    "_OptionalAutoMergingOutputTypeDef",
-    {
-        "Consolidation": ConsolidationOutputTypeDef,
-        "ConflictResolution": ConflictResolutionTypeDef,
-        "MinAllowedConfidenceScoreForMerging": float,
-    },
-    total=False,
-)
-
-
-class AutoMergingOutputTypeDef(
-    _RequiredAutoMergingOutputTypeDef, _OptionalAutoMergingOutputTypeDef
-):
-    pass
-
-
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1542,15 +1488,14 @@
 )
 
 
 class AutoMergingTypeDef(_RequiredAutoMergingTypeDef, _OptionalAutoMergingTypeDef):
     pass
 
 
-ConsolidationUnionTypeDef = Union[ConsolidationTypeDef, ConsolidationOutputTypeDef]
 _RequiredGetAutoMergingPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetAutoMergingPreviewRequestRequestTypeDef",
     {
         "DomainName": str,
         "Consolidation": ConsolidationTypeDef,
         "ConflictResolution": ConflictResolutionTypeDef,
     },
@@ -1792,15 +1737,15 @@
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1809,31 +1754,62 @@
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ObjectTypeName": str,
+        "Description": str,
+    },
+)
+_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "TemplateId": str,
+        "ExpirationDays": int,
+        "EncryptionKey": str,
+        "AllowProfileCreation": bool,
+        "SourceLastUpdatedTimestampFormat": str,
+        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
+        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class PutProfileObjectTypeRequestRequestTypeDef(
+    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
+    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
+):
+    pass
+
+
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1962,15 +1938,14 @@
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ObjectTypeKeyUnionTypeDef = Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Marketo": MarketoSourcePropertiesTypeDef,
         "S3": S3SourcePropertiesTypeDef,
         "Salesforce": SalesforceSourcePropertiesTypeDef,
         "ServiceNow": ServiceNowSourcePropertiesTypeDef,
@@ -2045,15 +2020,14 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeDetailsUnionTypeDef = Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef]
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2088,15 +2062,15 @@
 
 CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
         "Conditions": ConditionsTypeDef,
         "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2108,15 +2082,15 @@
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
@@ -2149,15 +2123,15 @@
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
@@ -2190,15 +2164,15 @@
 
 
 MatchingResponseTypeDef = TypedDict(
     "MatchingResponseTypeDef",
     {
         "Enabled": bool,
         "JobSchedule": JobScheduleTypeDef,
-        "AutoMerging": AutoMergingOutputTypeDef,
+        "AutoMerging": AutoMergingTypeDef,
         "ExportingConfig": ExportingConfigTypeDef,
     },
     total=False,
 )
 
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
@@ -2207,15 +2181,15 @@
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
-        "AutoMerging": AutoMergingOutputTypeDef,
+        "AutoMerging": AutoMergingTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
@@ -2238,45 +2212,14 @@
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "ObjectTypeName": str,
-        "Description": str,
-    },
-)
-_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "TemplateId": str,
-        "ExpirationDays": int,
-        "EncryptionKey": str,
-        "AllowProfileCreation": bool,
-        "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class PutProfileObjectTypeRequestRequestTypeDef(
-    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
-    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "ConnectorType": SourceConnectorTypeType,
         "SourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles/type_defs.pyi` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     "AdditionalSearchKeyTypeDef",
     "AddressTypeDef",
     "AppflowIntegrationWorkflowAttributesTypeDef",
     "AppflowIntegrationWorkflowMetricsTypeDef",
     "AppflowIntegrationWorkflowStepTypeDef",
     "AttributeItemTypeDef",
     "ConflictResolutionTypeDef",
-    "ConsolidationOutputTypeDef",
     "ConsolidationTypeDef",
     "TimestampTypeDef",
     "RangeTypeDef",
     "ThresholdTypeDef",
     "ConnectorOperatorTypeDef",
     "CreateEventStreamRequestRequestTypeDef",
     "DeleteCalculatedAttributeDefinitionRequestRequestTypeDef",
@@ -90,15 +89,15 @@
     "GetIdentityResolutionJobRequestRequestTypeDef",
     "JobStatsTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetMatchesRequestRequestTypeDef",
     "MatchItemTypeDef",
     "GetProfileObjectTypeRequestRequestTypeDef",
     "ObjectTypeFieldTypeDef",
-    "ObjectTypeKeyOutputTypeDef",
+    "ObjectTypeKeyTypeDef",
     "GetProfileObjectTypeTemplateRequestRequestTypeDef",
     "GetWorkflowRequestRequestTypeDef",
     "GetWorkflowStepsRequestRequestTypeDef",
     "IncrementalPullConfigTypeDef",
     "JobScheduleTypeDef",
     "ListAccountIntegrationsRequestRequestTypeDef",
     "ListIntegrationItemTypeDef",
@@ -117,15 +116,14 @@
     "ListProfileObjectTypeTemplatesRequestRequestTypeDef",
     "ListProfileObjectTypesRequestRequestTypeDef",
     "ListProfileObjectsItemTypeDef",
     "ObjectFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListWorkflowsItemTypeDef",
     "MarketoSourcePropertiesTypeDef",
-    "ObjectTypeKeyTypeDef",
     "PutProfileObjectRequestRequestTypeDef",
     "S3SourcePropertiesTypeDef",
     "SalesforceSourcePropertiesTypeDef",
     "ServiceNowSourcePropertiesTypeDef",
     "ZendeskSourcePropertiesTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
@@ -149,19 +147,16 @@
     "PutProfileObjectResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "SearchProfilesRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "WorkflowAttributesTypeDef",
     "WorkflowMetricsTypeDef",
     "WorkflowStepItemTypeDef",
-    "AttributeDetailsOutputTypeDef",
     "AttributeDetailsTypeDef",
-    "AutoMergingOutputTypeDef",
     "AutoMergingTypeDef",
-    "ConsolidationUnionTypeDef",
     "GetAutoMergingPreviewRequestRequestTypeDef",
     "BatchTypeDef",
     "ListWorkflowsRequestRequestTypeDef",
     "ScheduledTriggerPropertiesTypeDef",
     "ConditionsTypeDef",
     "TaskTypeDef",
     "EventStreamSummaryTypeDef",
@@ -169,45 +164,43 @@
     "ExportingConfigTypeDef",
     "ExportingLocationTypeDef",
     "MergeProfilesRequestRequestTypeDef",
     "ProfileTypeDef",
     "GetMatchesResponseTypeDef",
     "GetProfileObjectTypeResponseTypeDef",
     "GetProfileObjectTypeTemplateResponseTypeDef",
+    "PutProfileObjectTypeRequestRequestTypeDef",
     "PutProfileObjectTypeResponseTypeDef",
     "ListAccountIntegrationsResponseTypeDef",
     "ListIntegrationsResponseTypeDef",
     "ListCalculatedAttributeDefinitionsResponseTypeDef",
     "ListCalculatedAttributesForProfileResponseTypeDef",
     "ListDomainsResponseTypeDef",
     "ListEventStreamsRequestListEventStreamsPaginateTypeDef",
     "ListProfileObjectTypesResponseTypeDef",
     "ListProfileObjectTypeTemplatesResponseTypeDef",
     "ListProfileObjectsResponseTypeDef",
     "ListProfileObjectsRequestRequestTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "ObjectTypeKeyUnionTypeDef",
     "SourceConnectorPropertiesTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "GetWorkflowResponseTypeDef",
     "GetWorkflowStepsResponseTypeDef",
-    "AttributeDetailsUnionTypeDef",
     "TriggerPropertiesTypeDef",
     "CreateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     "GetCalculatedAttributeDefinitionResponseTypeDef",
     "UpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
     "UpdateCalculatedAttributeDefinitionResponseTypeDef",
     "ListEventStreamsResponseTypeDef",
     "MatchingRequestTypeDef",
     "MatchingResponseTypeDef",
     "GetIdentityResolutionJobResponseTypeDef",
     "IdentityResolutionJobTypeDef",
     "SearchProfilesResponseTypeDef",
-    "PutProfileObjectTypeRequestRequestTypeDef",
     "SourceFlowConfigTypeDef",
     "TriggerConfigTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainRequestRequestTypeDef",
     "CreateDomainResponseTypeDef",
     "GetDomainResponseTypeDef",
     "UpdateDomainResponseTypeDef",
@@ -331,21 +324,14 @@
 )
 
 class ConflictResolutionTypeDef(
     _RequiredConflictResolutionTypeDef, _OptionalConflictResolutionTypeDef
 ):
     pass
 
-ConsolidationOutputTypeDef = TypedDict(
-    "ConsolidationOutputTypeDef",
-    {
-        "MatchingAttributesList": List[List[str]],
-    },
-)
-
 ConsolidationTypeDef = TypedDict(
     "ConsolidationTypeDef",
     {
         "MatchingAttributesList": Sequence[Sequence[str]],
     },
 )
 
@@ -693,16 +679,16 @@
         "Source": str,
         "Target": str,
         "ContentType": FieldContentTypeType,
     },
     total=False,
 )
 
-ObjectTypeKeyOutputTypeDef = TypedDict(
-    "ObjectTypeKeyOutputTypeDef",
+ObjectTypeKeyTypeDef = TypedDict(
+    "ObjectTypeKeyTypeDef",
     {
         "StandardIdentifiers": List[StandardIdentifierType],
         "FieldNames": List[str],
     },
     total=False,
 )
 
@@ -1075,23 +1061,14 @@
 MarketoSourcePropertiesTypeDef = TypedDict(
     "MarketoSourcePropertiesTypeDef",
     {
         "Object": str,
     },
 )
 
-ObjectTypeKeyTypeDef = TypedDict(
-    "ObjectTypeKeyTypeDef",
-    {
-        "StandardIdentifiers": Sequence[StandardIdentifierType],
-        "FieldNames": Sequence[str],
-    },
-    total=False,
-)
-
 PutProfileObjectRequestRequestTypeDef = TypedDict(
     "PutProfileObjectRequestRequestTypeDef",
     {
         "ObjectTypeName": str,
         "Object": str,
         "DomainName": str,
     },
@@ -1437,51 +1414,22 @@
     "WorkflowStepItemTypeDef",
     {
         "AppflowIntegration": AppflowIntegrationWorkflowStepTypeDef,
     },
     total=False,
 )
 
-AttributeDetailsOutputTypeDef = TypedDict(
-    "AttributeDetailsOutputTypeDef",
-    {
-        "Attributes": List[AttributeItemTypeDef],
-        "Expression": str,
-    },
-)
-
 AttributeDetailsTypeDef = TypedDict(
     "AttributeDetailsTypeDef",
     {
         "Attributes": Sequence[AttributeItemTypeDef],
         "Expression": str,
     },
 )
 
-_RequiredAutoMergingOutputTypeDef = TypedDict(
-    "_RequiredAutoMergingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalAutoMergingOutputTypeDef = TypedDict(
-    "_OptionalAutoMergingOutputTypeDef",
-    {
-        "Consolidation": ConsolidationOutputTypeDef,
-        "ConflictResolution": ConflictResolutionTypeDef,
-        "MinAllowedConfidenceScoreForMerging": float,
-    },
-    total=False,
-)
-
-class AutoMergingOutputTypeDef(
-    _RequiredAutoMergingOutputTypeDef, _OptionalAutoMergingOutputTypeDef
-):
-    pass
-
 _RequiredAutoMergingTypeDef = TypedDict(
     "_RequiredAutoMergingTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalAutoMergingTypeDef = TypedDict(
@@ -1493,15 +1441,14 @@
     },
     total=False,
 )
 
 class AutoMergingTypeDef(_RequiredAutoMergingTypeDef, _OptionalAutoMergingTypeDef):
     pass
 
-ConsolidationUnionTypeDef = Union[ConsolidationTypeDef, ConsolidationOutputTypeDef]
 _RequiredGetAutoMergingPreviewRequestRequestTypeDef = TypedDict(
     "_RequiredGetAutoMergingPreviewRequestRequestTypeDef",
     {
         "DomainName": str,
         "Consolidation": ConsolidationTypeDef,
         "ConflictResolution": ConflictResolutionTypeDef,
     },
@@ -1731,15 +1678,15 @@
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1748,31 +1695,60 @@
     {
         "TemplateId": str,
         "SourceName": str,
         "SourceObject": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "ObjectTypeName": str,
+        "Description": str,
+    },
+)
+_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
+    {
+        "TemplateId": str,
+        "ExpirationDays": int,
+        "EncryptionKey": str,
+        "AllowProfileCreation": bool,
+        "SourceLastUpdatedTimestampFormat": str,
+        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
+        "Keys": Mapping[str, Sequence[ObjectTypeKeyTypeDef]],
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class PutProfileObjectTypeRequestRequestTypeDef(
+    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
+    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
+):
+    pass
+
 PutProfileObjectTypeResponseTypeDef = TypedDict(
     "PutProfileObjectTypeResponseTypeDef",
     {
         "ObjectTypeName": str,
         "Description": str,
         "TemplateId": str,
         "ExpirationDays": int,
         "EncryptionKey": str,
         "AllowProfileCreation": bool,
         "SourceLastUpdatedTimestampFormat": str,
         "Fields": Dict[str, ObjectTypeFieldTypeDef],
-        "Keys": Dict[str, List[ObjectTypeKeyOutputTypeDef]],
+        "Keys": Dict[str, List[ObjectTypeKeyTypeDef]],
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1897,15 +1873,14 @@
     {
         "Items": List[ListWorkflowsItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ObjectTypeKeyUnionTypeDef = Union[ObjectTypeKeyTypeDef, ObjectTypeKeyOutputTypeDef]
 SourceConnectorPropertiesTypeDef = TypedDict(
     "SourceConnectorPropertiesTypeDef",
     {
         "Marketo": MarketoSourcePropertiesTypeDef,
         "S3": S3SourcePropertiesTypeDef,
         "Salesforce": SalesforceSourcePropertiesTypeDef,
         "ServiceNow": ServiceNowSourcePropertiesTypeDef,
@@ -1978,15 +1953,14 @@
         "WorkflowType": Literal["APPFLOW_INTEGRATION"],
         "Items": List[WorkflowStepItemTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AttributeDetailsUnionTypeDef = Union[AttributeDetailsTypeDef, AttributeDetailsOutputTypeDef]
 TriggerPropertiesTypeDef = TypedDict(
     "TriggerPropertiesTypeDef",
     {
         "Scheduled": ScheduledTriggerPropertiesTypeDef,
     },
     total=False,
 )
@@ -2019,15 +1993,15 @@
 
 CreateCalculatedAttributeDefinitionResponseTypeDef = TypedDict(
     "CreateCalculatedAttributeDefinitionResponseTypeDef",
     {
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
         "Conditions": ConditionsTypeDef,
         "Statistic": StatisticType,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2039,15 +2013,15 @@
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCalculatedAttributeDefinitionRequestRequestTypeDef",
@@ -2078,15 +2052,15 @@
         "CalculatedAttributeName": str,
         "DisplayName": str,
         "Description": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "Statistic": StatisticType,
         "Conditions": ConditionsTypeDef,
-        "AttributeDetails": AttributeDetailsOutputTypeDef,
+        "AttributeDetails": AttributeDetailsTypeDef,
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventStreamsResponseTypeDef = TypedDict(
     "ListEventStreamsResponseTypeDef",
@@ -2117,15 +2091,15 @@
     pass
 
 MatchingResponseTypeDef = TypedDict(
     "MatchingResponseTypeDef",
     {
         "Enabled": bool,
         "JobSchedule": JobScheduleTypeDef,
-        "AutoMerging": AutoMergingOutputTypeDef,
+        "AutoMerging": AutoMergingTypeDef,
         "ExportingConfig": ExportingConfigTypeDef,
     },
     total=False,
 )
 
 GetIdentityResolutionJobResponseTypeDef = TypedDict(
     "GetIdentityResolutionJobResponseTypeDef",
@@ -2134,15 +2108,15 @@
         "JobId": str,
         "Status": IdentityResolutionJobStatusType,
         "Message": str,
         "JobStartTime": datetime,
         "JobEndTime": datetime,
         "LastUpdatedAt": datetime,
         "JobExpirationTime": datetime,
-        "AutoMerging": AutoMergingOutputTypeDef,
+        "AutoMerging": AutoMergingTypeDef,
         "ExportingLocation": ExportingLocationTypeDef,
         "JobStats": JobStatsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IdentityResolutionJobTypeDef = TypedDict(
@@ -2165,43 +2139,14 @@
     {
         "Items": List[ProfileTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "DomainName": str,
-        "ObjectTypeName": str,
-        "Description": str,
-    },
-)
-_OptionalPutProfileObjectTypeRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProfileObjectTypeRequestRequestTypeDef",
-    {
-        "TemplateId": str,
-        "ExpirationDays": int,
-        "EncryptionKey": str,
-        "AllowProfileCreation": bool,
-        "SourceLastUpdatedTimestampFormat": str,
-        "Fields": Mapping[str, ObjectTypeFieldTypeDef],
-        "Keys": Mapping[str, Sequence[ObjectTypeKeyUnionTypeDef]],
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class PutProfileObjectTypeRequestRequestTypeDef(
-    _RequiredPutProfileObjectTypeRequestRequestTypeDef,
-    _OptionalPutProfileObjectTypeRequestRequestTypeDef,
-):
-    pass
-
 _RequiredSourceFlowConfigTypeDef = TypedDict(
     "_RequiredSourceFlowConfigTypeDef",
     {
         "ConnectorType": SourceConnectorTypeType,
         "SourceConnectorProperties": SourceConnectorPropertiesTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-customer-profiles-2.5.2.post1/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt` & `types-aiobotocore-customer-profiles-2.5.2.post2/types_aiobotocore_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

