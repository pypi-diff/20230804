# Comparing `tmp/types-aiobotocore-shield-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-shield-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-shield-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-shield-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-shield-2.5.2.post1.tar` & `types-aiobotocore-shield-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.689455 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27511 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27464 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22928 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22909 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:45.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.693455 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:53:01.000000 types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13004 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11490 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2065 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      809 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      808 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      928 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27481 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27434 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9265 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9263 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3299 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3295 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22173 2023-08-04 13:53:42.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22154 2023-08-04 13:53:38.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:37.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.636643 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13004 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      794 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       25 2023-08-04 13:59:26.000000 types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/LICENSE` & `types-aiobotocore-shield-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post1/PKG-INFO` & `types-aiobotocore-shield-2.5.2.post2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,130 +289,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_shield.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Shield` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/literals/).
+
 ```python
-from types_aiobotocore_shield.literals import (
-    ApplicationLayerAutomaticResponseStatusType,
-    AttackLayerType,
-    AttackPropertyIdentifierType,
-    AutoRenewType,
-    ListAttacksPaginatorName,
-    ListProtectionsPaginatorName,
-    ProactiveEngagementStatusType,
-    ProtectedResourceTypeType,
-    ProtectionGroupAggregationType,
-    ProtectionGroupPatternType,
-    SubResourceTypeType,
-    SubscriptionStateType,
-    UnitType,
-    ShieldServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_shield.literals import ApplicationLayerAutomaticResponseStatusType
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_shield.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Shield` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/type_defs/).
+
 ```python
-from types_aiobotocore_shield.type_defs import (
-    ResponseActionOutputTypeDef,
-    AssociateDRTLogBucketRequestRequestTypeDef,
-    AssociateDRTRoleRequestRequestTypeDef,
-    AssociateHealthCheckRequestRequestTypeDef,
-    EmergencyContactTypeDef,
-    MitigationTypeDef,
-    SummarizedCounterTypeDef,
-    ContributorTypeDef,
-    AttackVectorDescriptionTypeDef,
-    AttackVolumeStatisticsTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteProtectionGroupRequestRequestTypeDef,
-    DeleteProtectionRequestRequestTypeDef,
-    DescribeAttackRequestRequestTypeDef,
-    TimeRangeOutputTypeDef,
-    DescribeProtectionGroupRequestRequestTypeDef,
-    ProtectionGroupTypeDef,
-    DescribeProtectionRequestRequestTypeDef,
-    DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    DisassociateDRTLogBucketRequestRequestTypeDef,
-    DisassociateHealthCheckRequestRequestTypeDef,
-    ResponseActionTypeDef,
-    InclusionProtectionFiltersTypeDef,
-    InclusionProtectionGroupFiltersTypeDef,
-    LimitTypeDef,
-    PaginatorConfigTypeDef,
-    ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ProtectionGroupArbitraryPatternLimitsTypeDef,
-    TimestampTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateProtectionGroupRequestRequestTypeDef,
-    UpdateSubscriptionRequestRequestTypeDef,
-    ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    UpdateEmergencyContactSettingsRequestRequestTypeDef,
-    SummarizedAttackVectorTypeDef,
-    AttackPropertyTypeDef,
-    AttackSummaryTypeDef,
-    AttackVolumeTypeDef,
-    CreateProtectionGroupRequestRequestTypeDef,
-    CreateProtectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateProtectionResponseTypeDef,
-    DescribeDRTAccessResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
-    GetSubscriptionStateResponseTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DescribeProtectionGroupResponseTypeDef,
-    ListProtectionGroupsResponseTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    ResponseActionUnionTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    ListProtectionsRequestRequestTypeDef,
-    ListProtectionGroupsRequestRequestTypeDef,
-    ProtectionLimitsTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
-    ProtectionGroupPatternTypeLimitsTypeDef,
-    TimeRangeTypeDef,
-    ProtectionTypeDef,
-    SubResourceSummaryTypeDef,
-    ListAttacksResponseTypeDef,
-    AttackStatisticsDataItemTypeDef,
-    ProtectionGroupLimitsTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
-    TimeRangeUnionTypeDef,
-    DescribeProtectionResponseTypeDef,
-    ListProtectionsResponseTypeDef,
-    AttackDetailTypeDef,
-    DescribeAttackStatisticsResponseTypeDef,
-    SubscriptionLimitsTypeDef,
-    DescribeAttackResponseTypeDef,
-    SubscriptionTypeDef,
-    DescribeSubscriptionResponseTypeDef,
-)
+from types_aiobotocore_shield.type_defs import ResponseActionTypeDef
 
 
-def get_value() -> ResponseActionOutputTypeDef:
+def get_value() -> ResponseActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/README.md` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-shield
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore shield type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-shield"></a>
 
 # types-aiobotocore-shield
 
 [![PyPI - types-aiobotocore-shield](https://img.shields.io/pypi/v/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
@@ -15,15 +47,15 @@
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,130 +289,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_shield.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Shield` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/literals/).
+
 ```python
-from types_aiobotocore_shield.literals import (
-    ApplicationLayerAutomaticResponseStatusType,
-    AttackLayerType,
-    AttackPropertyIdentifierType,
-    AutoRenewType,
-    ListAttacksPaginatorName,
-    ListProtectionsPaginatorName,
-    ProactiveEngagementStatusType,
-    ProtectedResourceTypeType,
-    ProtectionGroupAggregationType,
-    ProtectionGroupPatternType,
-    SubResourceTypeType,
-    SubscriptionStateType,
-    UnitType,
-    ShieldServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_shield.literals import ApplicationLayerAutomaticResponseStatusType
 
 
 def check_value(value: ApplicationLayerAutomaticResponseStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_shield.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Shield` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/type_defs/).
+
 ```python
-from types_aiobotocore_shield.type_defs import (
-    ResponseActionOutputTypeDef,
-    AssociateDRTLogBucketRequestRequestTypeDef,
-    AssociateDRTRoleRequestRequestTypeDef,
-    AssociateHealthCheckRequestRequestTypeDef,
-    EmergencyContactTypeDef,
-    MitigationTypeDef,
-    SummarizedCounterTypeDef,
-    ContributorTypeDef,
-    AttackVectorDescriptionTypeDef,
-    AttackVolumeStatisticsTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteProtectionGroupRequestRequestTypeDef,
-    DeleteProtectionRequestRequestTypeDef,
-    DescribeAttackRequestRequestTypeDef,
-    TimeRangeOutputTypeDef,
-    DescribeProtectionGroupRequestRequestTypeDef,
-    ProtectionGroupTypeDef,
-    DescribeProtectionRequestRequestTypeDef,
-    DisableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    DisassociateDRTLogBucketRequestRequestTypeDef,
-    DisassociateHealthCheckRequestRequestTypeDef,
-    ResponseActionTypeDef,
-    InclusionProtectionFiltersTypeDef,
-    InclusionProtectionGroupFiltersTypeDef,
-    LimitTypeDef,
-    PaginatorConfigTypeDef,
-    ListResourcesInProtectionGroupRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ProtectionGroupArbitraryPatternLimitsTypeDef,
-    TimestampTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateProtectionGroupRequestRequestTypeDef,
-    UpdateSubscriptionRequestRequestTypeDef,
-    ApplicationLayerAutomaticResponseConfigurationTypeDef,
-    AssociateProactiveEngagementDetailsRequestRequestTypeDef,
-    UpdateEmergencyContactSettingsRequestRequestTypeDef,
-    SummarizedAttackVectorTypeDef,
-    AttackPropertyTypeDef,
-    AttackSummaryTypeDef,
-    AttackVolumeTypeDef,
-    CreateProtectionGroupRequestRequestTypeDef,
-    CreateProtectionRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateProtectionResponseTypeDef,
-    DescribeDRTAccessResponseTypeDef,
-    DescribeEmergencyContactSettingsResponseTypeDef,
-    GetSubscriptionStateResponseTypeDef,
-    ListResourcesInProtectionGroupResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    DescribeProtectionGroupResponseTypeDef,
-    ListProtectionGroupsResponseTypeDef,
-    EnableApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    ResponseActionUnionTypeDef,
-    UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef,
-    ListProtectionsRequestRequestTypeDef,
-    ListProtectionGroupsRequestRequestTypeDef,
-    ProtectionLimitsTypeDef,
-    ListProtectionsRequestListProtectionsPaginateTypeDef,
-    ProtectionGroupPatternTypeLimitsTypeDef,
-    TimeRangeTypeDef,
-    ProtectionTypeDef,
-    SubResourceSummaryTypeDef,
-    ListAttacksResponseTypeDef,
-    AttackStatisticsDataItemTypeDef,
-    ProtectionGroupLimitsTypeDef,
-    ListAttacksRequestListAttacksPaginateTypeDef,
-    ListAttacksRequestRequestTypeDef,
-    TimeRangeUnionTypeDef,
-    DescribeProtectionResponseTypeDef,
-    ListProtectionsResponseTypeDef,
-    AttackDetailTypeDef,
-    DescribeAttackStatisticsResponseTypeDef,
-    SubscriptionLimitsTypeDef,
-    DescribeAttackResponseTypeDef,
-    SubscriptionTypeDef,
-    DescribeSubscriptionResponseTypeDef,
-)
+from types_aiobotocore_shield.type_defs import ResponseActionTypeDef
 
 
-def get_value() -> ResponseActionOutputTypeDef:
+def get_value() -> ResponseActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/setup.py` & `types-aiobotocore-shield-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-shield",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Shield 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.py` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__init__.pyi` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/__main__.py` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Shield 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Shield 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.py` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ResponseActionUnionTypeDef,
+    ResponseActionTypeDef,
     TagTypeDef,
-    TimeRangeUnionTypeDef,
+    TimeRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -332,15 +332,15 @@
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#disassociate_health_check)
         """
 
     async def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionTypeDef
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#enable_application_layer_automatic_response)
@@ -378,16 +378,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#get_subscription_state)
         """
 
     async def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeUnionTypeDef = ...,
-        EndTime: TimeRangeUnionTypeDef = ...,
+        StartTime: TimeRangeTypeDef = ...,
+        EndTime: TimeRangeTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -457,15 +457,15 @@
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#untag_resource)
         """
 
     async def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#update_application_layer_automatic_response)
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/client.pyi` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     InclusionProtectionFiltersTypeDef,
     InclusionProtectionGroupFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionGroupsResponseTypeDef,
     ListProtectionsResponseTypeDef,
     ListResourcesInProtectionGroupResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ResponseActionUnionTypeDef,
+    ResponseActionTypeDef,
     TagTypeDef,
-    TimeRangeUnionTypeDef,
+    TimeRangeTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -303,15 +303,15 @@
         Removes health-based detection from the Shield Advanced protection for a
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.disassociate_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#disassociate_health_check)
         """
     async def enable_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionTypeDef
     ) -> Dict[str, Any]:
         """
         Enable the Shield Advanced automatic application layer DDoS mitigation for the
         protected resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.enable_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#enable_application_layer_automatic_response)
@@ -345,16 +345,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.get_subscription_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#get_subscription_state)
         """
     async def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeUnionTypeDef = ...,
-        EndTime: TimeRangeUnionTypeDef = ...,
+        StartTime: TimeRangeTypeDef = ...,
+        EndTime: TimeRangeTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
@@ -417,15 +417,15 @@
         """
         Removes tags from a resource in Shield.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#untag_resource)
         """
     async def update_application_layer_automatic_response(
-        self, *, ResourceArn: str, Action: ResponseActionUnionTypeDef
+        self, *, ResourceArn: str, Action: ResponseActionTypeDef
     ) -> Dict[str, Any]:
         """
         Updates an existing Shield Advanced automatic application layer DDoS mitigation
         configuration for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_application_layer_automatic_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#update_application_layer_automatic_response)
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.py` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,15 @@
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
@@ -184,14 +185,15 @@
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
@@ -270,26 +272,28 @@
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

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/literals.pyi` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
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
@@ -182,14 +183,15 @@
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
@@ -268,26 +270,28 @@
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

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.py` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeUnionTypeDef,
+    TimeRangeTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
@@ -54,16 +54,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeUnionTypeDef = ...,
-        EndTime: TimeRangeUnionTypeDef = ...,
+        StartTime: TimeRangeTypeDef = ...,
+        EndTime: TimeRangeTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
         """
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/paginator.pyi` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     InclusionProtectionFiltersTypeDef,
     ListAttacksResponseTypeDef,
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
-    TimeRangeUnionTypeDef,
+    TimeRangeTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
@@ -51,16 +51,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
-        StartTime: TimeRangeUnionTypeDef = ...,
-        EndTime: TimeRangeUnionTypeDef = ...,
+        StartTime: TimeRangeTypeDef = ...,
+        EndTime: TimeRangeTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
         """
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.py` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for shield service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_shield.type_defs import ResponseActionOutputTypeDef
+    from types_aiobotocore_shield.type_defs import ResponseActionTypeDef
 
-    data: ResponseActionOutputTypeDef = ...
+    data: ResponseActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Sequence
 
 from .literals import (
     ApplicationLayerAutomaticResponseStatusType,
     AttackLayerType,
     AttackPropertyIdentifierType,
     AutoRenewType,
     ProactiveEngagementStatusType,
@@ -32,49 +32,49 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ResponseActionOutputTypeDef",
+    "ResponseActionTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
-    "TimeRangeOutputTypeDef",
+    "TimeRangeTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
-    "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
     "PaginatorConfigTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
-    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
@@ -82,45 +82,40 @@
     "TagResourceRequestRequestTypeDef",
     "CreateProtectionResponseTypeDef",
     "DescribeDRTAccessResponseTypeDef",
     "DescribeEmergencyContactSettingsResponseTypeDef",
     "GetSubscriptionStateResponseTypeDef",
     "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ListAttacksRequestRequestTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    "ResponseActionUnionTypeDef",
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
-    "TimeRangeTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
-    "TimeRangeUnionTypeDef",
     "DescribeProtectionResponseTypeDef",
     "ListProtectionsResponseTypeDef",
     "AttackDetailTypeDef",
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
     "DescribeSubscriptionResponseTypeDef",
 )
 
-ResponseActionOutputTypeDef = TypedDict(
-    "ResponseActionOutputTypeDef",
+ResponseActionTypeDef = TypedDict(
+    "ResponseActionTypeDef",
     {
         "Block": Dict[str, Any],
         "Count": Dict[str, Any],
     },
     total=False,
 )
 
@@ -247,16 +242,16 @@
 DescribeAttackRequestRequestTypeDef = TypedDict(
     "DescribeAttackRequestRequestTypeDef",
     {
         "AttackId": str,
     },
 )
 
-TimeRangeOutputTypeDef = TypedDict(
-    "TimeRangeOutputTypeDef",
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
@@ -317,23 +312,14 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
-ResponseActionTypeDef = TypedDict(
-    "ResponseActionTypeDef",
-    {
-        "Block": Mapping[str, Any],
-        "Count": Mapping[str, Any],
-    },
-    total=False,
-)
-
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
         "ResourceTypes": Sequence[ProtectedResourceTypeType],
     },
@@ -403,15 +389,14 @@
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -449,15 +434,31 @@
     total=False,
 )
 
 ApplicationLayerAutomaticResponseConfigurationTypeDef = TypedDict(
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     {
         "Status": ApplicationLayerAutomaticResponseStatusType,
-        "Action": ResponseActionOutputTypeDef,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
     },
 )
 
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
@@ -629,14 +630,26 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -646,31 +659,14 @@
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-ResponseActionUnionTypeDef = Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
-UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "InclusionFilters": InclusionProtectionFiltersTypeDef,
     },
@@ -690,14 +686,25 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
     {
         "InclusionFilters": InclusionProtectionFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -706,23 +713,14 @@
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "FromInclusive": TimestampTypeDef,
-        "ToExclusive": TimestampTypeDef,
-    },
-    total=False,
-)
-
 ProtectionTypeDef = TypedDict(
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
@@ -779,38 +777,14 @@
     "ProtectionGroupLimitsTypeDef",
     {
         "MaxProtectionGroups": int,
         "PatternTypeLimits": ProtectionGroupPatternTypeLimitsTypeDef,
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
-    {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -838,15 +812,15 @@
     },
     total=False,
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
-        "TimeRange": TimeRangeOutputTypeDef,
+        "TimeRange": TimeRangeTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield/type_defs.pyi` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for shield service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_shield.type_defs import ResponseActionOutputTypeDef
+    from types_aiobotocore_shield.type_defs import ResponseActionTypeDef
 
-    data: ResponseActionOutputTypeDef = ...
+    data: ResponseActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Sequence
 
 from .literals import (
     ApplicationLayerAutomaticResponseStatusType,
     AttackLayerType,
     AttackPropertyIdentifierType,
     AutoRenewType,
     ProactiveEngagementStatusType,
@@ -31,49 +31,49 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ResponseActionOutputTypeDef",
+    "ResponseActionTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
     "SummarizedCounterTypeDef",
     "ContributorTypeDef",
     "AttackVectorDescriptionTypeDef",
     "AttackVolumeStatisticsTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProtectionGroupRequestRequestTypeDef",
     "DeleteProtectionRequestRequestTypeDef",
     "DescribeAttackRequestRequestTypeDef",
-    "TimeRangeOutputTypeDef",
+    "TimeRangeTypeDef",
     "DescribeProtectionGroupRequestRequestTypeDef",
     "ProtectionGroupTypeDef",
     "DescribeProtectionRequestRequestTypeDef",
     "DisableApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "DisassociateDRTLogBucketRequestRequestTypeDef",
     "DisassociateHealthCheckRequestRequestTypeDef",
-    "ResponseActionTypeDef",
     "InclusionProtectionFiltersTypeDef",
     "InclusionProtectionGroupFiltersTypeDef",
     "LimitTypeDef",
     "PaginatorConfigTypeDef",
     "ListResourcesInProtectionGroupRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
-    "TimestampTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProtectionGroupRequestRequestTypeDef",
     "UpdateSubscriptionRequestRequestTypeDef",
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     "UpdateEmergencyContactSettingsRequestRequestTypeDef",
     "SummarizedAttackVectorTypeDef",
     "AttackPropertyTypeDef",
     "AttackSummaryTypeDef",
     "AttackVolumeTypeDef",
     "CreateProtectionGroupRequestRequestTypeDef",
@@ -81,45 +81,40 @@
     "TagResourceRequestRequestTypeDef",
     "CreateProtectionResponseTypeDef",
     "DescribeDRTAccessResponseTypeDef",
     "DescribeEmergencyContactSettingsResponseTypeDef",
     "GetSubscriptionStateResponseTypeDef",
     "ListResourcesInProtectionGroupResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ListAttacksRequestRequestTypeDef",
     "DescribeProtectionGroupResponseTypeDef",
     "ListProtectionGroupsResponseTypeDef",
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    "ResponseActionUnionTypeDef",
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
     "ListProtectionsRequestRequestTypeDef",
     "ListProtectionGroupsRequestRequestTypeDef",
     "ProtectionLimitsTypeDef",
+    "ListAttacksRequestListAttacksPaginateTypeDef",
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
     "ProtectionGroupPatternTypeLimitsTypeDef",
-    "TimeRangeTypeDef",
     "ProtectionTypeDef",
     "SubResourceSummaryTypeDef",
     "ListAttacksResponseTypeDef",
     "AttackStatisticsDataItemTypeDef",
     "ProtectionGroupLimitsTypeDef",
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    "ListAttacksRequestRequestTypeDef",
-    "TimeRangeUnionTypeDef",
     "DescribeProtectionResponseTypeDef",
     "ListProtectionsResponseTypeDef",
     "AttackDetailTypeDef",
     "DescribeAttackStatisticsResponseTypeDef",
     "SubscriptionLimitsTypeDef",
     "DescribeAttackResponseTypeDef",
     "SubscriptionTypeDef",
     "DescribeSubscriptionResponseTypeDef",
 )
 
-ResponseActionOutputTypeDef = TypedDict(
-    "ResponseActionOutputTypeDef",
+ResponseActionTypeDef = TypedDict(
+    "ResponseActionTypeDef",
     {
         "Block": Dict[str, Any],
         "Count": Dict[str, Any],
     },
     total=False,
 )
 
@@ -244,16 +239,16 @@
 DescribeAttackRequestRequestTypeDef = TypedDict(
     "DescribeAttackRequestRequestTypeDef",
     {
         "AttackId": str,
     },
 )
 
-TimeRangeOutputTypeDef = TypedDict(
-    "TimeRangeOutputTypeDef",
+TimeRangeTypeDef = TypedDict(
+    "TimeRangeTypeDef",
     {
         "FromInclusive": datetime,
         "ToExclusive": datetime,
     },
     total=False,
 )
 
@@ -312,23 +307,14 @@
     "DisassociateHealthCheckRequestRequestTypeDef",
     {
         "ProtectionId": str,
         "HealthCheckArn": str,
     },
 )
 
-ResponseActionTypeDef = TypedDict(
-    "ResponseActionTypeDef",
-    {
-        "Block": Mapping[str, Any],
-        "Count": Mapping[str, Any],
-    },
-    total=False,
-)
-
 InclusionProtectionFiltersTypeDef = TypedDict(
     "InclusionProtectionFiltersTypeDef",
     {
         "ResourceArns": Sequence[str],
         "ProtectionNames": Sequence[str],
         "ResourceTypes": Sequence[ProtectedResourceTypeType],
     },
@@ -396,15 +382,14 @@
 ProtectionGroupArbitraryPatternLimitsTypeDef = TypedDict(
     "ProtectionGroupArbitraryPatternLimitsTypeDef",
     {
         "MaxMembers": int,
     },
 )
 
-TimestampTypeDef = Union[datetime, str]
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -440,15 +425,31 @@
     total=False,
 )
 
 ApplicationLayerAutomaticResponseConfigurationTypeDef = TypedDict(
     "ApplicationLayerAutomaticResponseConfigurationTypeDef",
     {
         "Status": ApplicationLayerAutomaticResponseStatusType,
-        "Action": ResponseActionOutputTypeDef,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
+    },
+)
+
+UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
+    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "Action": ResponseActionTypeDef,
     },
 )
 
 AssociateProactiveEngagementDetailsRequestRequestTypeDef = TypedDict(
     "AssociateProactiveEngagementDetailsRequestRequestTypeDef",
     {
         "EmergencyContactList": Sequence[EmergencyContactTypeDef],
@@ -614,14 +615,26 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAttacksRequestRequestTypeDef = TypedDict(
+    "ListAttacksRequestRequestTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
 DescribeProtectionGroupResponseTypeDef = TypedDict(
     "DescribeProtectionGroupResponseTypeDef",
     {
         "ProtectionGroup": ProtectionGroupTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -631,31 +644,14 @@
     {
         "ProtectionGroups": List[ProtectionGroupTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EnableApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "EnableApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
-ResponseActionUnionTypeDef = Union[ResponseActionTypeDef, ResponseActionOutputTypeDef]
-UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef = TypedDict(
-    "UpdateApplicationLayerAutomaticResponseRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "Action": ResponseActionTypeDef,
-    },
-)
-
 ListProtectionsRequestRequestTypeDef = TypedDict(
     "ListProtectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "InclusionFilters": InclusionProtectionFiltersTypeDef,
     },
@@ -675,14 +671,25 @@
 ProtectionLimitsTypeDef = TypedDict(
     "ProtectionLimitsTypeDef",
     {
         "ProtectedResourceTypeLimits": List[LimitTypeDef],
     },
 )
 
+ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
+    "ListAttacksRequestListAttacksPaginateTypeDef",
+    {
+        "ResourceArns": Sequence[str],
+        "StartTime": TimeRangeTypeDef,
+        "EndTime": TimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProtectionsRequestListProtectionsPaginateTypeDef = TypedDict(
     "ListProtectionsRequestListProtectionsPaginateTypeDef",
     {
         "InclusionFilters": InclusionProtectionFiltersTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -691,23 +698,14 @@
 ProtectionGroupPatternTypeLimitsTypeDef = TypedDict(
     "ProtectionGroupPatternTypeLimitsTypeDef",
     {
         "ArbitraryPatternLimits": ProtectionGroupArbitraryPatternLimitsTypeDef,
     },
 )
 
-TimeRangeTypeDef = TypedDict(
-    "TimeRangeTypeDef",
-    {
-        "FromInclusive": TimestampTypeDef,
-        "ToExclusive": TimestampTypeDef,
-    },
-    total=False,
-)
-
 ProtectionTypeDef = TypedDict(
     "ProtectionTypeDef",
     {
         "Id": str,
         "Name": str,
         "ResourceArn": str,
         "HealthCheckIds": List[str],
@@ -762,38 +760,14 @@
     "ProtectionGroupLimitsTypeDef",
     {
         "MaxProtectionGroups": int,
         "PatternTypeLimits": ProtectionGroupPatternTypeLimitsTypeDef,
     },
 )
 
-ListAttacksRequestListAttacksPaginateTypeDef = TypedDict(
-    "ListAttacksRequestListAttacksPaginateTypeDef",
-    {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListAttacksRequestRequestTypeDef = TypedDict(
-    "ListAttacksRequestRequestTypeDef",
-    {
-        "ResourceArns": Sequence[str],
-        "StartTime": TimeRangeTypeDef,
-        "EndTime": TimeRangeTypeDef,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-TimeRangeUnionTypeDef = Union[TimeRangeTypeDef, TimeRangeOutputTypeDef]
 DescribeProtectionResponseTypeDef = TypedDict(
     "DescribeProtectionResponseTypeDef",
     {
         "Protection": ProtectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -821,15 +795,15 @@
     },
     total=False,
 )
 
 DescribeAttackStatisticsResponseTypeDef = TypedDict(
     "DescribeAttackStatisticsResponseTypeDef",
     {
-        "TimeRange": TimeRangeOutputTypeDef,
+        "TimeRange": TimeRangeTypeDef,
         "DataItems": List[AttackStatisticsDataItemTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SubscriptionLimitsTypeDef = TypedDict(
     "SubscriptionLimitsTypeDef",
```

### Comparing `types-aiobotocore-shield-2.5.2.post1/types_aiobotocore_shield.egg-info/SOURCES.txt` & `types-aiobotocore-shield-2.5.2.post2/types_aiobotocore_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

