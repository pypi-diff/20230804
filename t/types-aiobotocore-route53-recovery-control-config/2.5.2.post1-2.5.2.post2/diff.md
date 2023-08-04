# Comparing `tmp/types-aiobotocore-route53-recovery-control-config-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-route53-recovery-control-config-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-control-config-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-control-config-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1.tar` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17854 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25723 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25680 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9366 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23234 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23203 2023-08-02 14:48:07.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.789475 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19465 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16550 2023-08-04 13:59:23.826643 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14939 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.826643 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2240 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2985 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2984 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1033 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25723 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25680 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9461 2023-08-04 13:51:09.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9459 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7497 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7490 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23234 2023-08-04 13:51:09.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23203 2023-08-04 13:51:09.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7506 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7500 2023-08-04 13:51:08.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16550 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1390 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       50 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/LICENSE` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/PKG-INFO` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-route53-recovery-control-config
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53-recovery-control-config type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,118 +324,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_route53_recovery_control_config.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `Route53RecoveryControlConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/literals/).
+
 ```python
-from types_aiobotocore_route53_recovery_control_config.literals import (
-    ClusterCreatedWaiterName,
-    ClusterDeletedWaiterName,
-    ControlPanelCreatedWaiterName,
-    ControlPanelDeletedWaiterName,
-    ListAssociatedRoute53HealthChecksPaginatorName,
-    ListClustersPaginatorName,
-    ListControlPanelsPaginatorName,
-    ListRoutingControlsPaginatorName,
-    ListSafetyRulesPaginatorName,
-    RoutingControlCreatedWaiterName,
-    RoutingControlDeletedWaiterName,
-    RuleTypeType,
-    StatusType,
-    Route53RecoveryControlConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-)
+from types_aiobotocore_route53_recovery_control_config.literals import ClusterCreatedWaiterName
 
 
 def check_value(value: ClusterCreatedWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_route53_recovery_control_config.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `Route53RecoveryControlConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/type_defs/).
+
 ```python
-from types_aiobotocore_route53_recovery_control_config.type_defs import (
-    RuleConfigTypeDef,
-    AssertionRuleUpdateTypeDef,
-    ClusterEndpointTypeDef,
-    ControlPanelTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateControlPanelRequestRequestTypeDef,
-    CreateRoutingControlRequestRequestTypeDef,
-    RoutingControlTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteControlPanelRequestRequestTypeDef,
-    DeleteRoutingControlRequestRequestTypeDef,
-    DeleteSafetyRuleRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeClusterRequestRequestTypeDef,
-    DescribeControlPanelRequestRequestTypeDef,
-    DescribeRoutingControlRequestRequestTypeDef,
-    DescribeSafetyRuleRequestRequestTypeDef,
-    GatingRuleUpdateTypeDef,
-    PaginatorConfigTypeDef,
-    ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
-    ListClustersRequestRequestTypeDef,
-    ListControlPanelsRequestRequestTypeDef,
-    ListRoutingControlsRequestRequestTypeDef,
-    ListSafetyRulesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateControlPanelRequestRequestTypeDef,
-    UpdateRoutingControlRequestRequestTypeDef,
-    AssertionRuleTypeDef,
-    GatingRuleTypeDef,
-    NewAssertionRuleTypeDef,
-    NewGatingRuleTypeDef,
-    ClusterTypeDef,
-    CreateControlPanelResponseTypeDef,
-    DescribeControlPanelResponseTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
-    ListControlPanelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateControlPanelResponseTypeDef,
-    CreateRoutingControlResponseTypeDef,
-    DescribeRoutingControlResponseTypeDef,
-    ListRoutingControlsResponseTypeDef,
-    UpdateRoutingControlResponseTypeDef,
-    DescribeClusterRequestClusterCreatedWaitTypeDef,
-    DescribeClusterRequestClusterDeletedWaitTypeDef,
-    DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
-    DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
-    DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
-    DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
-    UpdateSafetyRuleRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    CreateSafetyRuleResponseTypeDef,
-    DescribeSafetyRuleResponseTypeDef,
-    RuleTypeDef,
-    UpdateSafetyRuleResponseTypeDef,
-    CreateSafetyRuleRequestRequestTypeDef,
-    CreateClusterResponseTypeDef,
-    DescribeClusterResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListSafetyRulesResponseTypeDef,
-)
+from types_aiobotocore_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
 
 def get_value() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/README.md` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-route53-recovery-control-config
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore route53-recovery-control-config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53-recovery-control-config"></a>
 
 # types-aiobotocore-route53-recovery-control-config
 
 [![PyPI - types-aiobotocore-route53-recovery-control-config](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-control-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/)
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,118 +356,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_route53_recovery_control_config.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `Route53RecoveryControlConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/literals/).
+
 ```python
-from types_aiobotocore_route53_recovery_control_config.literals import (
-    ClusterCreatedWaiterName,
-    ClusterDeletedWaiterName,
-    ControlPanelCreatedWaiterName,
-    ControlPanelDeletedWaiterName,
-    ListAssociatedRoute53HealthChecksPaginatorName,
-    ListClustersPaginatorName,
-    ListControlPanelsPaginatorName,
-    ListRoutingControlsPaginatorName,
-    ListSafetyRulesPaginatorName,
-    RoutingControlCreatedWaiterName,
-    RoutingControlDeletedWaiterName,
-    RuleTypeType,
-    StatusType,
-    Route53RecoveryControlConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-)
+from types_aiobotocore_route53_recovery_control_config.literals import ClusterCreatedWaiterName
 
 
 def check_value(value: ClusterCreatedWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_route53_recovery_control_config.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `Route53RecoveryControlConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/type_defs/).
+
 ```python
-from types_aiobotocore_route53_recovery_control_config.type_defs import (
-    RuleConfigTypeDef,
-    AssertionRuleUpdateTypeDef,
-    ClusterEndpointTypeDef,
-    ControlPanelTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateControlPanelRequestRequestTypeDef,
-    CreateRoutingControlRequestRequestTypeDef,
-    RoutingControlTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteControlPanelRequestRequestTypeDef,
-    DeleteRoutingControlRequestRequestTypeDef,
-    DeleteSafetyRuleRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeClusterRequestRequestTypeDef,
-    DescribeControlPanelRequestRequestTypeDef,
-    DescribeRoutingControlRequestRequestTypeDef,
-    DescribeSafetyRuleRequestRequestTypeDef,
-    GatingRuleUpdateTypeDef,
-    PaginatorConfigTypeDef,
-    ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
-    ListClustersRequestRequestTypeDef,
-    ListControlPanelsRequestRequestTypeDef,
-    ListRoutingControlsRequestRequestTypeDef,
-    ListSafetyRulesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateControlPanelRequestRequestTypeDef,
-    UpdateRoutingControlRequestRequestTypeDef,
-    AssertionRuleTypeDef,
-    GatingRuleTypeDef,
-    NewAssertionRuleTypeDef,
-    NewGatingRuleTypeDef,
-    ClusterTypeDef,
-    CreateControlPanelResponseTypeDef,
-    DescribeControlPanelResponseTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
-    ListControlPanelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateControlPanelResponseTypeDef,
-    CreateRoutingControlResponseTypeDef,
-    DescribeRoutingControlResponseTypeDef,
-    ListRoutingControlsResponseTypeDef,
-    UpdateRoutingControlResponseTypeDef,
-    DescribeClusterRequestClusterCreatedWaitTypeDef,
-    DescribeClusterRequestClusterDeletedWaitTypeDef,
-    DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
-    DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
-    DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
-    DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
-    UpdateSafetyRuleRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    CreateSafetyRuleResponseTypeDef,
-    DescribeSafetyRuleResponseTypeDef,
-    RuleTypeDef,
-    UpdateSafetyRuleResponseTypeDef,
-    CreateSafetyRuleRequestRequestTypeDef,
-    CreateClusterResponseTypeDef,
-    DescribeClusterResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListSafetyRulesResponseTypeDef,
-)
+from types_aiobotocore_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
 
 def get_value() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/setup.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-control-config",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_route53_recovery_control_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__init__.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/__main__.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#Route53RecoveryControlConfig\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/client.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ClusterCreatedWaiterName",
     "ClusterDeletedWaiterName",
     "ControlPanelCreatedWaiterName",
     "ControlPanelDeletedWaiterName",
     "ListAssociatedRoute53HealthChecksPaginatorName",
     "ListClustersPaginatorName",
@@ -36,15 +35,14 @@
     "Route53RecoveryControlConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
-
 ClusterCreatedWaiterName = Literal["cluster_created"]
 ClusterDeletedWaiterName = Literal["cluster_deleted"]
 ControlPanelCreatedWaiterName = Literal["control_panel_created"]
 ControlPanelDeletedWaiterName = Literal["control_panel_deleted"]
 ListAssociatedRoute53HealthChecksPaginatorName = Literal["list_associated_route53_health_checks"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListControlPanelsPaginatorName = Literal["list_control_panels"]
@@ -66,14 +64,15 @@
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
@@ -169,14 +168,15 @@
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
@@ -255,26 +255,28 @@
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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/literals.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ClusterCreatedWaiterName",
     "ClusterDeletedWaiterName",
     "ControlPanelCreatedWaiterName",
     "ControlPanelDeletedWaiterName",
     "ListAssociatedRoute53HealthChecksPaginatorName",
     "ListClustersPaginatorName",
@@ -35,14 +36,15 @@
     "Route53RecoveryControlConfigServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
+
 ClusterCreatedWaiterName = Literal["cluster_created"]
 ClusterDeletedWaiterName = Literal["cluster_deleted"]
 ControlPanelCreatedWaiterName = Literal["control_panel_created"]
 ControlPanelDeletedWaiterName = Literal["control_panel_deleted"]
 ListAssociatedRoute53HealthChecksPaginatorName = Literal["list_associated_route53_health_checks"]
 ListClustersPaginatorName = Literal["list_clusters"]
 ListControlPanelsPaginatorName = Literal["list_control_panels"]
@@ -64,14 +66,15 @@
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
@@ -167,14 +170,15 @@
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
@@ -253,26 +257,28 @@
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

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/paginator.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/type_defs.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.py` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config/waiter.pyi` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-control-config
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Route53RecoveryControlConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/
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
 [types-aiobotocore-route53-recovery-control-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -356,118 +356,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_route53_recovery_control_config.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `Route53RecoveryControlConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/literals/).
+
 ```python
-from types_aiobotocore_route53_recovery_control_config.literals import (
-    ClusterCreatedWaiterName,
-    ClusterDeletedWaiterName,
-    ControlPanelCreatedWaiterName,
-    ControlPanelDeletedWaiterName,
-    ListAssociatedRoute53HealthChecksPaginatorName,
-    ListClustersPaginatorName,
-    ListControlPanelsPaginatorName,
-    ListRoutingControlsPaginatorName,
-    ListSafetyRulesPaginatorName,
-    RoutingControlCreatedWaiterName,
-    RoutingControlDeletedWaiterName,
-    RuleTypeType,
-    StatusType,
-    Route53RecoveryControlConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-)
+from types_aiobotocore_route53_recovery_control_config.literals import ClusterCreatedWaiterName
 
 
 def check_value(value: ClusterCreatedWaiterName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_route53_recovery_control_config.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `Route53RecoveryControlConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_control_config/type_defs/).
+
 ```python
-from types_aiobotocore_route53_recovery_control_config.type_defs import (
-    RuleConfigTypeDef,
-    AssertionRuleUpdateTypeDef,
-    ClusterEndpointTypeDef,
-    ControlPanelTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateControlPanelRequestRequestTypeDef,
-    CreateRoutingControlRequestRequestTypeDef,
-    RoutingControlTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteControlPanelRequestRequestTypeDef,
-    DeleteRoutingControlRequestRequestTypeDef,
-    DeleteSafetyRuleRequestRequestTypeDef,
-    WaiterConfigTypeDef,
-    DescribeClusterRequestRequestTypeDef,
-    DescribeControlPanelRequestRequestTypeDef,
-    DescribeRoutingControlRequestRequestTypeDef,
-    DescribeSafetyRuleRequestRequestTypeDef,
-    GatingRuleUpdateTypeDef,
-    PaginatorConfigTypeDef,
-    ListAssociatedRoute53HealthChecksRequestRequestTypeDef,
-    ListClustersRequestRequestTypeDef,
-    ListControlPanelsRequestRequestTypeDef,
-    ListRoutingControlsRequestRequestTypeDef,
-    ListSafetyRulesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateControlPanelRequestRequestTypeDef,
-    UpdateRoutingControlRequestRequestTypeDef,
-    AssertionRuleTypeDef,
-    GatingRuleTypeDef,
-    NewAssertionRuleTypeDef,
-    NewGatingRuleTypeDef,
-    ClusterTypeDef,
-    CreateControlPanelResponseTypeDef,
-    DescribeControlPanelResponseTypeDef,
-    ListAssociatedRoute53HealthChecksResponseTypeDef,
-    ListControlPanelsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    UpdateControlPanelResponseTypeDef,
-    CreateRoutingControlResponseTypeDef,
-    DescribeRoutingControlResponseTypeDef,
-    ListRoutingControlsResponseTypeDef,
-    UpdateRoutingControlResponseTypeDef,
-    DescribeClusterRequestClusterCreatedWaitTypeDef,
-    DescribeClusterRequestClusterDeletedWaitTypeDef,
-    DescribeControlPanelRequestControlPanelCreatedWaitTypeDef,
-    DescribeControlPanelRequestControlPanelDeletedWaitTypeDef,
-    DescribeRoutingControlRequestRoutingControlCreatedWaitTypeDef,
-    DescribeRoutingControlRequestRoutingControlDeletedWaitTypeDef,
-    UpdateSafetyRuleRequestRequestTypeDef,
-    ListAssociatedRoute53HealthChecksRequestListAssociatedRoute53HealthChecksPaginateTypeDef,
-    ListClustersRequestListClustersPaginateTypeDef,
-    ListControlPanelsRequestListControlPanelsPaginateTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListSafetyRulesRequestListSafetyRulesPaginateTypeDef,
-    CreateSafetyRuleResponseTypeDef,
-    DescribeSafetyRuleResponseTypeDef,
-    RuleTypeDef,
-    UpdateSafetyRuleResponseTypeDef,
-    CreateSafetyRuleRequestRequestTypeDef,
-    CreateClusterResponseTypeDef,
-    DescribeClusterResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListSafetyRulesResponseTypeDef,
-)
+from types_aiobotocore_route53_recovery_control_config.type_defs import RuleConfigTypeDef
 
 
 def get_value() -> RuleConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-route53-recovery-control-config-2.5.2.post1/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-control-config-2.5.2.post2/types_aiobotocore_route53_recovery_control_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

