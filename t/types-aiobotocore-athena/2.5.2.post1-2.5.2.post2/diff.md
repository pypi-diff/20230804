# Comparing `tmp/types-aiobotocore-athena-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-athena-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-athena-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-athena-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-athena-2.5.2.post1.tar` & `types-aiobotocore-athena-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19895 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:33:30.000000 types-aiobotocore-athena-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.069648 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48924 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48840 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63863 2023-08-02 14:33:33.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63772 2023-08-02 14:33:32.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.087217 types-aiobotocore-athena-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-08-04 12:00:28.087217 types-aiobotocore-athena-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12283 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.087217 types-aiobotocore-athena-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.083217 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48904 2023-08-04 11:40:41.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-08-04 11:40:41.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-08-04 11:40:41.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-04 11:40:41.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-08-04 11:40:41.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-04 11:40:41.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    62716 2023-08-04 11:40:43.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62627 2023-08-04 11:40:42.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:40.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.087217 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13797 2023-08-04 12:00:27.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:27.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:27.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:27.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:27.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:27.000000 types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-athena-2.5.2.post1/LICENSE` & `types-aiobotocore-athena-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/setup.py` & `types-aiobotocore-athena-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-athena",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.py` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.pyi` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__main__.py` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Athena 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Athena 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.py` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentUnionTypeDef,
+    CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationUnionTypeDef,
+    EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -730,15 +730,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_work_groups)
         """
 
     async def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef]
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#put_capacity_assignment_configuration)
@@ -778,15 +778,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_query_execution)
         """
 
     async def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationUnionTypeDef,
+        EngineConfiguration: EngineConfigurationTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.pyi` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentUnionTypeDef,
+    CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationUnionTypeDef,
+    EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -670,15 +670,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_work_groups)
         """
     async def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef]
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#put_capacity_assignment_configuration)
@@ -715,15 +715,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_query_execution)
         """
     async def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationUnionTypeDef,
+        EngineConfiguration: EngineConfigurationTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.py` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.pyi` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.py` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.pyi` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.py` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_athena.type_defs import AclConfigurationTypeDef
 
     data: AclConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -55,15 +55,14 @@
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
-    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
     "CreateNotebookInputRequestTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
@@ -76,15 +75,14 @@
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
@@ -162,30 +160,29 @@
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "CapacityAssignmentUnionTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
-    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
@@ -204,15 +201,14 @@
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -419,26 +415,18 @@
 
 class CapacityAllocationTypeDef(
     _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
 ):
     pass
 
 
-CapacityAssignmentOutputTypeDef = TypedDict(
-    "CapacityAssignmentOutputTypeDef",
-    {
-        "WorkGroupNames": List[str],
-    },
-    total=False,
-)
-
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": Sequence[str],
+        "WorkGroupNames": List[str],
     },
     total=False,
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
@@ -712,51 +700,27 @@
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
 
-_RequiredEngineConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEngineConfigurationOutputTypeDef",
-    {
-        "MaxConcurrentDpus": int,
-    },
-)
-_OptionalEngineConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEngineConfigurationOutputTypeDef",
-    {
-        "CoordinatorDpuSize": int,
-        "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Dict[str, str],
-        "SparkProperties": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class EngineConfigurationOutputTypeDef(
-    _RequiredEngineConfigurationOutputTypeDef, _OptionalEngineConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEngineConfigurationTypeDef = TypedDict(
     "_RequiredEngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
     },
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Mapping[str, str],
-        "SparkProperties": Mapping[str, str],
+        "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
     },
     total=False,
 )
 
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
@@ -1766,20 +1730,27 @@
     pass
 
 
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
+        "CapacityAssignments": List[CapacityAssignmentTypeDef],
     },
     total=False,
 )
 
-CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
+    },
+)
+
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1947,17 +1918,14 @@
         "WorkingDirectory": str,
         "IdleTimeoutSeconds": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-EngineConfigurationUnionTypeDef = Union[
-    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
-]
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2278,22 +2246,14 @@
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
-    },
-)
-
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2355,15 +2315,15 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "SessionId": str,
         "Description": str,
         "WorkGroup": str,
         "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "EngineConfiguration": EngineConfigurationTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.pyi` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_athena.type_defs import AclConfigurationTypeDef
 
     data: AclConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -54,15 +54,14 @@
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
-    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
     "CreateNotebookInputRequestTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
@@ -75,15 +74,14 @@
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
@@ -161,30 +159,29 @@
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "CapacityAssignmentUnionTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
-    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
@@ -203,15 +200,14 @@
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -414,26 +410,18 @@
 )
 
 class CapacityAllocationTypeDef(
     _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
 ):
     pass
 
-CapacityAssignmentOutputTypeDef = TypedDict(
-    "CapacityAssignmentOutputTypeDef",
-    {
-        "WorkGroupNames": List[str],
-    },
-    total=False,
-)
-
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": Sequence[str],
+        "WorkGroupNames": List[str],
     },
     total=False,
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
@@ -689,49 +677,27 @@
 )
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
-_RequiredEngineConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEngineConfigurationOutputTypeDef",
-    {
-        "MaxConcurrentDpus": int,
-    },
-)
-_OptionalEngineConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEngineConfigurationOutputTypeDef",
-    {
-        "CoordinatorDpuSize": int,
-        "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Dict[str, str],
-        "SparkProperties": Dict[str, str],
-    },
-    total=False,
-)
-
-class EngineConfigurationOutputTypeDef(
-    _RequiredEngineConfigurationOutputTypeDef, _OptionalEngineConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredEngineConfigurationTypeDef = TypedDict(
     "_RequiredEngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
     },
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Mapping[str, str],
-        "SparkProperties": Mapping[str, str],
+        "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
     },
     total=False,
 )
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
@@ -1701,20 +1667,27 @@
 ):
     pass
 
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
+        "CapacityAssignments": List[CapacityAssignmentTypeDef],
     },
     total=False,
 )
 
-CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
+    },
+)
+
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1876,17 +1849,14 @@
         "WorkingDirectory": str,
         "IdleTimeoutSeconds": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
-EngineConfigurationUnionTypeDef = Union[
-    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
-]
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2195,22 +2165,14 @@
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
-    },
-)
-
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2272,15 +2234,15 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "SessionId": str,
         "Description": str,
         "WorkGroup": str,
         "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "EngineConfiguration": EngineConfigurationTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/SOURCES.txt` & `types-aiobotocore-athena-2.5.2.post2/types_aiobotocore_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

