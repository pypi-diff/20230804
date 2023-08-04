# Comparing `tmp/types-aiobotocore-cleanrooms-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cleanrooms-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cleanrooms-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-cleanrooms-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cleanrooms-2.5.2.post1.tar` & `types-aiobotocore-cleanrooms-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.853637 types-aiobotocore-cleanrooms-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-08-02 14:51:59.849637 types-aiobotocore-cleanrooms-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.853637 types-aiobotocore-cleanrooms-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31981 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    31928 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-08-02 14:34:17.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43244 2023-08-02 14:34:18.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43189 2023-08-02 14:34:18.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:16.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19490 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:51:59.000000 types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.171409 types-aiobotocore-cleanrooms-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-04 12:00:33.167408 types-aiobotocore-cleanrooms-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12575 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.171409 types-aiobotocore-cleanrooms-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-04 11:41:29.000000 types-aiobotocore-cleanrooms-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.151408 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31966 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31913 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    41235 2023-08-04 11:41:31.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41182 2023-08-04 11:41:31.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:30.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.167408 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-04 12:00:32.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:32.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:32.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:32.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:32.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:32.000000 types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/LICENSE` & `types-aiobotocore-cleanrooms-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/setup.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cleanrooms",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CleanRoomsService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__init__.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/__main__.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CleanRoomsService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
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

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
     BatchGetSchemaOutputTypeDef,
-    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
+    ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
     GetCollaborationOutputTypeDef,
@@ -185,15 +185,15 @@
         """
 
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -527,15 +527,15 @@
         """
 
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/client.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     ListMembershipsPaginator,
     ListMembersPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 from .type_defs import (
     BatchGetSchemaOutputTypeDef,
-    ConfiguredTableAnalysisRulePolicyUnionTypeDef,
+    ConfiguredTableAnalysisRulePolicyTypeDef,
     CreateCollaborationOutputTypeDef,
     CreateConfiguredTableAnalysisRuleOutputTypeDef,
     CreateConfiguredTableAssociationOutputTypeDef,
     CreateConfiguredTableOutputTypeDef,
     CreateMembershipOutputTypeDef,
     DataEncryptionMetadataTypeDef,
     GetCollaborationOutputTypeDef,
@@ -175,15 +175,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table)
         """
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -486,15 +486,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table)
         """
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/literals.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/paginator.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.py` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for cleanrooms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnOutputTypeDef
+    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnTypeDef
 
-    data: AggregateColumnOutputTypeDef = ...
+    data: AggregateColumnTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
@@ -37,18 +37,16 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
-    "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
@@ -95,15 +93,14 @@
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
-    "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
@@ -125,55 +122,44 @@
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
-    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
-    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
     "UpdateConfiguredTableOutputTypeDef",
     "StartProtectedQueryInputRequestTypeDef",
     "ProtectedQueryTypeDef",
     "AnalysisRuleTypeDef",
     "ConfiguredTableAnalysisRuleTypeDef",
-    "ConfiguredTableAnalysisRulePolicyUnionTypeDef",
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "UpdateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetProtectedQueryOutputTypeDef",
     "StartProtectedQueryOutputTypeDef",
     "UpdateProtectedQueryOutputTypeDef",
     "GetSchemaAnalysisRuleOutputTypeDef",
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
 )
 
-AggregateColumnOutputTypeDef = TypedDict(
-    "AggregateColumnOutputTypeDef",
-    {
-        "columnNames": List[str],
-        "function": AggregateFunctionNameType,
-    },
-)
-
 AggregateColumnTypeDef = TypedDict(
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
@@ -183,22 +169,14 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
-AnalysisRuleListOutputTypeDef = TypedDict(
-    "AnalysisRuleListOutputTypeDef",
-    {
-        "joinColumns": List[str],
-        "listColumns": List[str],
-    },
-)
-
 AnalysisRuleListTypeDef = TypedDict(
     "AnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
@@ -906,39 +884,14 @@
     {
         "membershipIdentifier": str,
         "protectedQueryIdentifier": str,
         "targetStatus": Literal["CANCELLED"],
     },
 )
 
-_RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
-    "_RequiredAnalysisRuleAggregationOutputTypeDef",
-    {
-        "aggregateColumns": List[AggregateColumnOutputTypeDef],
-        "joinColumns": List[str],
-        "dimensionColumns": List[str],
-        "scalarFunctions": List[ScalarFunctionsType],
-        "outputConstraints": List[AggregationConstraintTypeDef],
-    },
-)
-_OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
-    "_OptionalAnalysisRuleAggregationOutputTypeDef",
-    {
-        "joinRequired": Literal["QUERY_RUNNER"],
-    },
-    total=False,
-)
-
-
-class AnalysisRuleAggregationOutputTypeDef(
-    _RequiredAnalysisRuleAggregationOutputTypeDef, _OptionalAnalysisRuleAggregationOutputTypeDef
-):
-    pass
-
-
 _RequiredAnalysisRuleAggregationTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationTypeDef",
     {
         "aggregateColumns": Sequence[AggregateColumnTypeDef],
         "joinColumns": Sequence[str],
         "dimensionColumns": Sequence[str],
         "scalarFunctions": Sequence[ScalarFunctionsType],
@@ -1304,25 +1257,16 @@
     },
     total=False,
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
-        "list": AnalysisRuleListOutputTypeDef,
-        "aggregation": AnalysisRuleAggregationOutputTypeDef,
-    },
-    total=False,
-)
-
-ConfiguredTableAnalysisRulePolicyV1OutputTypeDef = TypedDict(
-    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
-    {
-        "list": AnalysisRuleListOutputTypeDef,
-        "aggregation": AnalysisRuleAggregationOutputTypeDef,
+        "list": AnalysisRuleListTypeDef,
+        "aggregation": AnalysisRuleAggregationTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
@@ -1444,22 +1388,14 @@
     "AnalysisRulePolicyTypeDef",
     {
         "v1": AnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
-ConfiguredTableAnalysisRulePolicyOutputTypeDef = TypedDict(
-    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
-    {
-        "v1": ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
-    },
-    total=False,
-)
-
 ConfiguredTableAnalysisRulePolicyTypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     {
         "v1": ConfiguredTableAnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
@@ -1538,24 +1474,21 @@
 )
 
 ConfiguredTableAnalysisRuleTypeDef = TypedDict(
     "ConfiguredTableAnalysisRuleTypeDef",
     {
         "configuredTableId": str,
         "configuredTableArn": str,
-        "policy": ConfiguredTableAnalysisRulePolicyOutputTypeDef,
+        "policy": ConfiguredTableAnalysisRulePolicyTypeDef,
         "type": ConfiguredTableAnalysisRuleTypeType,
         "createTime": datetime,
         "updateTime": datetime,
     },
 )
 
-ConfiguredTableAnalysisRulePolicyUnionTypeDef = Union[
-    ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
-]
 CreateConfiguredTableAnalysisRuleInputRequestTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     {
         "configuredTableIdentifier": str,
         "analysisRuleType": ConfiguredTableAnalysisRuleTypeType,
         "analysisRulePolicy": ConfiguredTableAnalysisRulePolicyTypeDef,
     },
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms/type_defs.pyi` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for cleanrooms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnOutputTypeDef
+    from types_aiobotocore_cleanrooms.type_defs import AggregateColumnTypeDef
 
-    data: AggregateColumnOutputTypeDef = ...
+    data: AggregateColumnTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AggregateFunctionNameType,
     AnalysisRuleTypeType,
     CollaborationQueryLogStatusType,
     ConfiguredTableAnalysisRuleTypeType,
     FilterableMemberStatusType,
@@ -36,18 +36,16 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AggregateColumnOutputTypeDef",
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
-    "AnalysisRuleListOutputTypeDef",
     "AnalysisRuleListTypeDef",
     "BatchGetSchemaErrorTypeDef",
     "BatchGetSchemaInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CollaborationSummaryTypeDef",
     "DataEncryptionMetadataTypeDef",
     "ColumnTypeDef",
@@ -94,15 +92,14 @@
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCollaborationInputRequestTypeDef",
     "UpdateConfiguredTableAssociationInputRequestTypeDef",
     "UpdateConfiguredTableInputRequestTypeDef",
     "UpdateMembershipInputRequestTypeDef",
     "UpdateProtectedQueryInputRequestTypeDef",
-    "AnalysisRuleAggregationOutputTypeDef",
     "AnalysisRuleAggregationTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListCollaborationsOutputTypeDef",
     "CollaborationTypeDef",
     "SchemaTypeDef",
     "ListConfiguredTableAssociationsOutputTypeDef",
     "CreateConfiguredTableAssociationOutputTypeDef",
@@ -124,55 +121,44 @@
     "ListMembersOutputTypeDef",
     "ListMembershipsOutputTypeDef",
     "ListProtectedQueriesOutputTypeDef",
     "ListSchemasOutputTypeDef",
     "ProtectedQueryOutputConfigurationTypeDef",
     "ProtectedQueryOutputTypeDef",
     "AnalysisRulePolicyV1TypeDef",
-    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     "CreateCollaborationOutputTypeDef",
     "GetCollaborationOutputTypeDef",
     "UpdateCollaborationOutputTypeDef",
     "BatchGetSchemaOutputTypeDef",
     "GetSchemaOutputTypeDef",
     "ConfiguredTableTypeDef",
     "CreateConfiguredTableInputRequestTypeDef",
     "ProtectedQueryResultConfigurationTypeDef",
     "ProtectedQueryResultTypeDef",
     "AnalysisRulePolicyTypeDef",
-    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     "CreateConfiguredTableOutputTypeDef",
     "GetConfiguredTableOutputTypeDef",
     "UpdateConfiguredTableOutputTypeDef",
     "StartProtectedQueryInputRequestTypeDef",
     "ProtectedQueryTypeDef",
     "AnalysisRuleTypeDef",
     "ConfiguredTableAnalysisRuleTypeDef",
-    "ConfiguredTableAnalysisRulePolicyUnionTypeDef",
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "UpdateConfiguredTableAnalysisRuleInputRequestTypeDef",
     "GetProtectedQueryOutputTypeDef",
     "StartProtectedQueryOutputTypeDef",
     "UpdateProtectedQueryOutputTypeDef",
     "GetSchemaAnalysisRuleOutputTypeDef",
     "CreateConfiguredTableAnalysisRuleOutputTypeDef",
     "GetConfiguredTableAnalysisRuleOutputTypeDef",
     "UpdateConfiguredTableAnalysisRuleOutputTypeDef",
 )
 
-AggregateColumnOutputTypeDef = TypedDict(
-    "AggregateColumnOutputTypeDef",
-    {
-        "columnNames": List[str],
-        "function": AggregateFunctionNameType,
-    },
-)
-
 AggregateColumnTypeDef = TypedDict(
     "AggregateColumnTypeDef",
     {
         "columnNames": Sequence[str],
         "function": AggregateFunctionNameType,
     },
 )
@@ -182,22 +168,14 @@
     {
         "columnName": str,
         "minimum": int,
         "type": Literal["COUNT_DISTINCT"],
     },
 )
 
-AnalysisRuleListOutputTypeDef = TypedDict(
-    "AnalysisRuleListOutputTypeDef",
-    {
-        "joinColumns": List[str],
-        "listColumns": List[str],
-    },
-)
-
 AnalysisRuleListTypeDef = TypedDict(
     "AnalysisRuleListTypeDef",
     {
         "joinColumns": Sequence[str],
         "listColumns": Sequence[str],
     },
 )
@@ -875,37 +853,14 @@
     {
         "membershipIdentifier": str,
         "protectedQueryIdentifier": str,
         "targetStatus": Literal["CANCELLED"],
     },
 )
 
-_RequiredAnalysisRuleAggregationOutputTypeDef = TypedDict(
-    "_RequiredAnalysisRuleAggregationOutputTypeDef",
-    {
-        "aggregateColumns": List[AggregateColumnOutputTypeDef],
-        "joinColumns": List[str],
-        "dimensionColumns": List[str],
-        "scalarFunctions": List[ScalarFunctionsType],
-        "outputConstraints": List[AggregationConstraintTypeDef],
-    },
-)
-_OptionalAnalysisRuleAggregationOutputTypeDef = TypedDict(
-    "_OptionalAnalysisRuleAggregationOutputTypeDef",
-    {
-        "joinRequired": Literal["QUERY_RUNNER"],
-    },
-    total=False,
-)
-
-class AnalysisRuleAggregationOutputTypeDef(
-    _RequiredAnalysisRuleAggregationOutputTypeDef, _OptionalAnalysisRuleAggregationOutputTypeDef
-):
-    pass
-
 _RequiredAnalysisRuleAggregationTypeDef = TypedDict(
     "_RequiredAnalysisRuleAggregationTypeDef",
     {
         "aggregateColumns": Sequence[AggregateColumnTypeDef],
         "joinColumns": Sequence[str],
         "dimensionColumns": Sequence[str],
         "scalarFunctions": Sequence[ScalarFunctionsType],
@@ -1255,25 +1210,16 @@
     },
     total=False,
 )
 
 AnalysisRulePolicyV1TypeDef = TypedDict(
     "AnalysisRulePolicyV1TypeDef",
     {
-        "list": AnalysisRuleListOutputTypeDef,
-        "aggregation": AnalysisRuleAggregationOutputTypeDef,
-    },
-    total=False,
-)
-
-ConfiguredTableAnalysisRulePolicyV1OutputTypeDef = TypedDict(
-    "ConfiguredTableAnalysisRulePolicyV1OutputTypeDef",
-    {
-        "list": AnalysisRuleListOutputTypeDef,
-        "aggregation": AnalysisRuleAggregationOutputTypeDef,
+        "list": AnalysisRuleListTypeDef,
+        "aggregation": AnalysisRuleAggregationTypeDef,
     },
     total=False,
 )
 
 ConfiguredTableAnalysisRulePolicyV1TypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyV1TypeDef",
     {
@@ -1391,22 +1337,14 @@
     "AnalysisRulePolicyTypeDef",
     {
         "v1": AnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
 
-ConfiguredTableAnalysisRulePolicyOutputTypeDef = TypedDict(
-    "ConfiguredTableAnalysisRulePolicyOutputTypeDef",
-    {
-        "v1": ConfiguredTableAnalysisRulePolicyV1OutputTypeDef,
-    },
-    total=False,
-)
-
 ConfiguredTableAnalysisRulePolicyTypeDef = TypedDict(
     "ConfiguredTableAnalysisRulePolicyTypeDef",
     {
         "v1": ConfiguredTableAnalysisRulePolicyV1TypeDef,
     },
     total=False,
 )
@@ -1483,24 +1421,21 @@
 )
 
 ConfiguredTableAnalysisRuleTypeDef = TypedDict(
     "ConfiguredTableAnalysisRuleTypeDef",
     {
         "configuredTableId": str,
         "configuredTableArn": str,
-        "policy": ConfiguredTableAnalysisRulePolicyOutputTypeDef,
+        "policy": ConfiguredTableAnalysisRulePolicyTypeDef,
         "type": ConfiguredTableAnalysisRuleTypeType,
         "createTime": datetime,
         "updateTime": datetime,
     },
 )
 
-ConfiguredTableAnalysisRulePolicyUnionTypeDef = Union[
-    ConfiguredTableAnalysisRulePolicyTypeDef, ConfiguredTableAnalysisRulePolicyOutputTypeDef
-]
 CreateConfiguredTableAnalysisRuleInputRequestTypeDef = TypedDict(
     "CreateConfiguredTableAnalysisRuleInputRequestTypeDef",
     {
         "configuredTableIdentifier": str,
         "analysisRuleType": ConfiguredTableAnalysisRuleTypeType,
         "analysisRulePolicy": ConfiguredTableAnalysisRulePolicyTypeDef,
     },
```

### Comparing `types-aiobotocore-cleanrooms-2.5.2.post1/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt` & `types-aiobotocore-cleanrooms-2.5.2.post2/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

