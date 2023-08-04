# Comparing `tmp/types-aiobotocore-auditmanager-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-auditmanager-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-auditmanager-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-auditmanager-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-auditmanager-2.5.2.post1.tar` & `types-aiobotocore-auditmanager-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18287 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45855 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45785 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58050 2023-08-02 14:33:35.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58005 2023-08-02 14:33:35.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:34.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.101648 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:51:54.000000 types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.111218 types-aiobotocore-auditmanager-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-04 12:00:28.111218 types-aiobotocore-auditmanager-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10905 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.111218 types-aiobotocore-auditmanager-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.107217 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45840 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45770 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-08-04 11:40:45.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57739 2023-08-04 11:40:47.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57694 2023-08-04 11:40:45.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:44.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.111218 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-08-04 12:00:27.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-04 12:00:27.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:27.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:27.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:27.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:27.000000 types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/LICENSE` & `types-aiobotocore-auditmanager-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/setup.py` & `types-aiobotocore-auditmanager-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-auditmanager",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_auditmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AuditManager 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/__main__.py` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AuditManager 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.AuditManager 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager\nOther"
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

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.py` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
-    ScopeUnionTypeDef,
+    ScopeTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentResponseTypeDef,
@@ -221,15 +221,15 @@
         """
 
     async def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: ScopeUnionTypeDef,
+        scope: ScopeTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -741,15 +741,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#untag_resource)
         """
 
     async def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: ScopeUnionTypeDef,
+        scope: ScopeTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/client.pyi` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     ListKeywordsForDataSourceResponseTypeDef,
     ListNotificationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ManualEvidenceTypeDef,
     RegisterAccountResponseTypeDef,
     RegisterOrganizationAdminAccountResponseTypeDef,
     RoleTypeDef,
-    ScopeUnionTypeDef,
+    ScopeTypeDef,
     StartAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentControlResponseTypeDef,
     UpdateAssessmentControlSetStatusResponseTypeDef,
     UpdateAssessmentFrameworkControlSetTypeDef,
     UpdateAssessmentFrameworkResponseTypeDef,
     UpdateAssessmentFrameworkShareResponseTypeDef,
     UpdateAssessmentResponseTypeDef,
@@ -209,15 +209,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#close)
         """
     async def create_assessment(
         self,
         *,
         name: str,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef,
-        scope: ScopeUnionTypeDef,
+        scope: ScopeTypeDef,
         roles: Sequence[RoleTypeDef],
         frameworkId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateAssessmentResponseTypeDef:
         """
         Creates an assessment in Audit Manager.
@@ -681,15 +681,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#AuditManager.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_auditmanager/client/#untag_resource)
         """
     async def update_assessment(
         self,
         *,
         assessmentId: str,
-        scope: ScopeUnionTypeDef,
+        scope: ScopeTypeDef,
         assessmentName: str = ...,
         assessmentDescription: str = ...,
         assessmentReportsDestination: AssessmentReportsDestinationTypeDef = ...,
         roles: Sequence[RoleTypeDef] = ...
     ) -> UpdateAssessmentResponseTypeDef:
         """
         Edits an Audit Manager assessment.
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.py` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/literals.pyi` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.py` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_auditmanager.type_defs import AWSAccountTypeDef
 
     data: AWSAccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountStatusType,
     ActionEnumType,
     AssessmentReportStatusType,
     AssessmentStatusType,
     ControlResponseType,
@@ -128,15 +128,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
-    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
     "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
     "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
     "CreateAssessmentReportResponseTypeDef",
     "DeregisterAccountResponseTypeDef",
@@ -177,15 +176,14 @@
     "GetAssessmentReportUrlResponseTypeDef",
     "GetInsightsByAssessmentResponseTypeDef",
     "GetInsightsResponseTypeDef",
     "GetServicesInScopeResponseTypeDef",
     "ListNotificationsResponseTypeDef",
     "AssessmentMetadataTypeDef",
     "CreateAssessmentRequestRequestTypeDef",
-    "ScopeUnionTypeDef",
     "UpdateAssessmentRequestRequestTypeDef",
     "ListAssessmentsResponseTypeDef",
     "AssessmentControlSetTypeDef",
     "UpdateAssessmentControlResponseTypeDef",
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
@@ -1207,23 +1205,14 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
-ScopeOutputTypeDef = TypedDict(
-    "ScopeOutputTypeDef",
-    {
-        "awsAccounts": List[AWSAccountTypeDef],
-        "awsServices": List[AWSServiceTypeDef],
-    },
-    total=False,
-)
-
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
     },
     total=False,
@@ -1715,15 +1704,15 @@
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
         "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "scope": ScopeOutputTypeDef,
+        "scope": ScopeTypeDef,
         "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
@@ -1750,15 +1739,14 @@
 
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
 
-ScopeUnionTypeDef = Union[ScopeTypeDef, ScopeOutputTypeDef]
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager/type_defs.pyi` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_auditmanager.type_defs import AWSAccountTypeDef
 
     data: AWSAccountTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountStatusType,
     ActionEnumType,
     AssessmentReportStatusType,
     AssessmentStatusType,
     ControlResponseType,
@@ -127,15 +127,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAssessmentControlRequestRequestTypeDef",
     "UpdateAssessmentControlSetStatusRequestRequestTypeDef",
     "UpdateAssessmentFrameworkShareRequestRequestTypeDef",
     "UpdateAssessmentStatusRequestRequestTypeDef",
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
-    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "AssessmentMetadataItemTypeDef",
     "AssessmentControlTypeDef",
     "BatchAssociateAssessmentReportEvidenceResponseTypeDef",
     "BatchDisassociateAssessmentReportEvidenceResponseTypeDef",
     "CreateAssessmentReportResponseTypeDef",
     "DeregisterAccountResponseTypeDef",
@@ -176,15 +175,14 @@
     "GetAssessmentReportUrlResponseTypeDef",
     "GetInsightsByAssessmentResponseTypeDef",
     "GetInsightsResponseTypeDef",
     "GetServicesInScopeResponseTypeDef",
     "ListNotificationsResponseTypeDef",
     "AssessmentMetadataTypeDef",
     "CreateAssessmentRequestRequestTypeDef",
-    "ScopeUnionTypeDef",
     "UpdateAssessmentRequestRequestTypeDef",
     "ListAssessmentsResponseTypeDef",
     "AssessmentControlSetTypeDef",
     "UpdateAssessmentControlResponseTypeDef",
     "BatchCreateDelegationByAssessmentResponseTypeDef",
     "BatchImportEvidenceToAssessmentControlResponseTypeDef",
     "ListControlDomainInsightsByAssessmentResponseTypeDef",
@@ -1178,23 +1176,14 @@
 ValidateAssessmentReportIntegrityRequestRequestTypeDef = TypedDict(
     "ValidateAssessmentReportIntegrityRequestRequestTypeDef",
     {
         "s3RelativePath": str,
     },
 )
 
-ScopeOutputTypeDef = TypedDict(
-    "ScopeOutputTypeDef",
-    {
-        "awsAccounts": List[AWSAccountTypeDef],
-        "awsServices": List[AWSServiceTypeDef],
-    },
-    total=False,
-)
-
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
         "awsAccounts": Sequence[AWSAccountTypeDef],
         "awsServices": Sequence[AWSServiceTypeDef],
     },
     total=False,
@@ -1682,15 +1671,15 @@
     {
         "name": str,
         "id": str,
         "description": str,
         "complianceType": str,
         "status": AssessmentStatusType,
         "assessmentReportsDestination": AssessmentReportsDestinationTypeDef,
-        "scope": ScopeOutputTypeDef,
+        "scope": ScopeTypeDef,
         "roles": List[RoleTypeDef],
         "delegations": List[DelegationTypeDef],
         "creationTime": datetime,
         "lastUpdated": datetime,
     },
     total=False,
 )
@@ -1715,15 +1704,14 @@
 )
 
 class CreateAssessmentRequestRequestTypeDef(
     _RequiredCreateAssessmentRequestRequestTypeDef, _OptionalCreateAssessmentRequestRequestTypeDef
 ):
     pass
 
-ScopeUnionTypeDef = Union[ScopeTypeDef, ScopeOutputTypeDef]
 _RequiredUpdateAssessmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
         "scope": ScopeTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-auditmanager-2.5.2.post1/types_aiobotocore_auditmanager.egg-info/SOURCES.txt` & `types-aiobotocore-auditmanager-2.5.2.post2/types_aiobotocore_auditmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

