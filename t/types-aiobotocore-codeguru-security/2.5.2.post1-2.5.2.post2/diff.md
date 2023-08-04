# Comparing `tmp/types-aiobotocore-codeguru-security-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codeguru-security-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-security-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-security-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-security-2.5.2.post1.tar` & `types-aiobotocore-codeguru-security-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.673624 types-aiobotocore-codeguru-security-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-02 14:52:02.669624 types-aiobotocore-codeguru-security-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13784 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.673624 types-aiobotocore-codeguru-security-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.661625 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-02 14:35:10.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-08-02 14:35:09.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.669624 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.679541 types-aiobotocore-codeguru-security-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-08-04 12:00:36.679541 types-aiobotocore-codeguru-security-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12214 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.679541 types-aiobotocore-codeguru-security-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.679541 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14227 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-08-04 11:42:26.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-08-04 11:42:26.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-08-04 11:42:26.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-08-04 11:42:26.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14774 2023-08-04 11:42:26.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.679541 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/LICENSE` & `types-aiobotocore-codeguru-security-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/PKG-INFO` & `types-aiobotocore-codeguru-security-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,93 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguru_security.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruSecurity` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/literals/).
+
 ```python
-from types_aiobotocore_codeguru_security.literals import (
-    AnalysisTypeType,
-    ErrorCodeType,
-    GetFindingsPaginatorName,
-    ListFindingsMetricsPaginatorName,
-    ListScansPaginatorName,
-    ScanStateType,
-    ScanTypeType,
-    SeverityType,
-    StatusType,
-    CodeGuruSecurityServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_codeguru_security.literals import AnalysisTypeType
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguru_security.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruSecurity` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/type_defs/).
+
 ```python
-from types_aiobotocore_codeguru_security.type_defs import (
-    FindingMetricsValuePerSeverityTypeDef,
-    BatchGetFindingsErrorTypeDef,
-    FindingIdentifierTypeDef,
-    ResponseMetadataTypeDef,
-    CategoryWithFindingNumTypeDef,
-    CodeLineTypeDef,
-    ResourceIdTypeDef,
-    CreateUploadUrlRequestRequestTypeDef,
-    EncryptionConfigTypeDef,
-    ResourceTypeDef,
-    PaginatorConfigTypeDef,
-    GetFindingsRequestRequestTypeDef,
-    TimestampTypeDef,
-    GetScanRequestRequestTypeDef,
-    ListScansRequestRequestTypeDef,
-    ScanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ScanNameWithFindingNumTypeDef,
-    RecommendationTypeDef,
-    SuggestedFixTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AccountFindingsMetricTypeDef,
-    BatchGetFindingsRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
-    GetScanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    FilePathTypeDef,
-    CreateScanRequestRequestTypeDef,
-    CreateScanResponseTypeDef,
-    GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
-    ListScansResponseTypeDef,
-    MetricsSummaryTypeDef,
-    RemediationTypeDef,
-    ListFindingsMetricsResponseTypeDef,
-    VulnerabilityTypeDef,
-    GetMetricsSummaryResponseTypeDef,
-    FindingTypeDef,
-    BatchGetFindingsResponseTypeDef,
-    GetFindingsResponseTypeDef,
-)
+from types_aiobotocore_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
 
 def get_value() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/README.md` & `types-aiobotocore-codeguru-security-2.5.2.post2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,93 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguru_security.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruSecurity` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/literals/).
+
 ```python
-from types_aiobotocore_codeguru_security.literals import (
-    AnalysisTypeType,
-    ErrorCodeType,
-    GetFindingsPaginatorName,
-    ListFindingsMetricsPaginatorName,
-    ListScansPaginatorName,
-    ScanStateType,
-    ScanTypeType,
-    SeverityType,
-    StatusType,
-    CodeGuruSecurityServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_codeguru_security.literals import AnalysisTypeType
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguru_security.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruSecurity` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/type_defs/).
+
 ```python
-from types_aiobotocore_codeguru_security.type_defs import (
-    FindingMetricsValuePerSeverityTypeDef,
-    BatchGetFindingsErrorTypeDef,
-    FindingIdentifierTypeDef,
-    ResponseMetadataTypeDef,
-    CategoryWithFindingNumTypeDef,
-    CodeLineTypeDef,
-    ResourceIdTypeDef,
-    CreateUploadUrlRequestRequestTypeDef,
-    EncryptionConfigTypeDef,
-    ResourceTypeDef,
-    PaginatorConfigTypeDef,
-    GetFindingsRequestRequestTypeDef,
-    TimestampTypeDef,
-    GetScanRequestRequestTypeDef,
-    ListScansRequestRequestTypeDef,
-    ScanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ScanNameWithFindingNumTypeDef,
-    RecommendationTypeDef,
-    SuggestedFixTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AccountFindingsMetricTypeDef,
-    BatchGetFindingsRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
-    GetScanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    FilePathTypeDef,
-    CreateScanRequestRequestTypeDef,
-    CreateScanResponseTypeDef,
-    GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
-    ListScansResponseTypeDef,
-    MetricsSummaryTypeDef,
-    RemediationTypeDef,
-    ListFindingsMetricsResponseTypeDef,
-    VulnerabilityTypeDef,
-    GetMetricsSummaryResponseTypeDef,
-    FindingTypeDef,
-    BatchGetFindingsResponseTypeDef,
-    GetFindingsResponseTypeDef,
-)
+from types_aiobotocore_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
 
 def get_value() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/setup.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-security",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codeguru_security"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__init__.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/__main__.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeGuruSecurity 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity\nOther"
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

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/client.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/literals.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/paginator.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.py` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security/type_defs.pyi` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-security
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeGuruSecurity 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-codeguru-security docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,93 +297,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguru_security.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruSecurity` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/literals/).
+
 ```python
-from types_aiobotocore_codeguru_security.literals import (
-    AnalysisTypeType,
-    ErrorCodeType,
-    GetFindingsPaginatorName,
-    ListFindingsMetricsPaginatorName,
-    ListScansPaginatorName,
-    ScanStateType,
-    ScanTypeType,
-    SeverityType,
-    StatusType,
-    CodeGuruSecurityServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_codeguru_security.literals import AnalysisTypeType
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguru_security.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruSecurity` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_security/type_defs/).
+
 ```python
-from types_aiobotocore_codeguru_security.type_defs import (
-    FindingMetricsValuePerSeverityTypeDef,
-    BatchGetFindingsErrorTypeDef,
-    FindingIdentifierTypeDef,
-    ResponseMetadataTypeDef,
-    CategoryWithFindingNumTypeDef,
-    CodeLineTypeDef,
-    ResourceIdTypeDef,
-    CreateUploadUrlRequestRequestTypeDef,
-    EncryptionConfigTypeDef,
-    ResourceTypeDef,
-    PaginatorConfigTypeDef,
-    GetFindingsRequestRequestTypeDef,
-    TimestampTypeDef,
-    GetScanRequestRequestTypeDef,
-    ListScansRequestRequestTypeDef,
-    ScanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ScanNameWithFindingNumTypeDef,
-    RecommendationTypeDef,
-    SuggestedFixTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AccountFindingsMetricTypeDef,
-    BatchGetFindingsRequestRequestTypeDef,
-    CreateUploadUrlResponseTypeDef,
-    GetScanResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    FilePathTypeDef,
-    CreateScanRequestRequestTypeDef,
-    CreateScanResponseTypeDef,
-    GetAccountConfigurationResponseTypeDef,
-    UpdateAccountConfigurationRequestRequestTypeDef,
-    UpdateAccountConfigurationResponseTypeDef,
-    GetFindingsRequestGetFindingsPaginateTypeDef,
-    ListScansRequestListScansPaginateTypeDef,
-    GetMetricsSummaryRequestRequestTypeDef,
-    ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef,
-    ListFindingsMetricsRequestRequestTypeDef,
-    ListScansResponseTypeDef,
-    MetricsSummaryTypeDef,
-    RemediationTypeDef,
-    ListFindingsMetricsResponseTypeDef,
-    VulnerabilityTypeDef,
-    GetMetricsSummaryResponseTypeDef,
-    FindingTypeDef,
-    BatchGetFindingsResponseTypeDef,
-    GetFindingsResponseTypeDef,
-)
+from types_aiobotocore_codeguru_security.type_defs import FindingMetricsValuePerSeverityTypeDef
 
 
 def get_value() -> FindingMetricsValuePerSeverityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codeguru-security-2.5.2.post1/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-security-2.5.2.post2/types_aiobotocore_codeguru_security.egg-info/SOURCES.txt`

 * *Files identical despite different names*

