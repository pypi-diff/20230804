# Comparing `tmp/types-aiobotocore-application-autoscaling-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-application-autoscaling-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-autoscaling-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-autoscaling-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:25 2023, max compression
```

## Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1.tar` & `types-aiobotocore-application-autoscaling-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15249 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17842 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26558 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26509 2023-08-02 14:33:13.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:12.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.729654 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16830 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:51:52.000000 types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.463112 types-aiobotocore-application-autoscaling-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-08-04 12:00:25.459112 types-aiobotocore-application-autoscaling-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:25.463112 types-aiobotocore-application-autoscaling-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-08-04 11:40:20.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.459112 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17796 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22793 2023-08-04 11:40:22.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:21.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.459112 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14423 2023-08-04 12:00:25.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-04 12:00:25.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:25.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 12:00:25.000000 types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/LICENSE` & `types-aiobotocore-application-autoscaling-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/PKG-INFO` & `types-aiobotocore-application-autoscaling-2.5.2.post2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-application-autoscaling
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,104 +305,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_application_autoscaling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApplicationAutoScaling` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/literals/).
+
 ```python
-from types_aiobotocore_application_autoscaling.literals import (
-    AdjustmentTypeType,
-    DescribeScalableTargetsPaginatorName,
-    DescribeScalingActivitiesPaginatorName,
-    DescribeScalingPoliciesPaginatorName,
-    DescribeScheduledActionsPaginatorName,
-    MetricAggregationTypeType,
-    MetricStatisticType,
-    MetricTypeType,
-    PolicyTypeType,
-    ScalableDimensionType,
-    ScalingActivityStatusCodeType,
-    ServiceNamespaceType,
-    ApplicationAutoScalingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_application_autoscaling.literals import AdjustmentTypeType
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_application_autoscaling.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApplicationAutoScaling` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/type_defs/).
+
 ```python
-from types_aiobotocore_application_autoscaling.type_defs import (
-    AlarmTypeDef,
-    MetricDimensionTypeDef,
-    DeleteScalingPolicyRequestRequestTypeDef,
-    DeleteScheduledActionRequestRequestTypeDef,
-    DeregisterScalableTargetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeScalableTargetsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NotScaledReasonTypeDef,
-    PredefinedMetricSpecificationTypeDef,
-    ScalableTargetActionTypeDef,
-    TimestampTypeDef,
-    SuspendedStateTypeDef,
-    StepAdjustmentTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TargetTrackingMetricDimensionTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutScalingPolicyResponseTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ScalingActivityTypeDef,
-    ScheduledActionTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
-    RegisterScalableTargetRequestRequestTypeDef,
-    ScalableTargetTypeDef,
-    StepScalingPolicyConfigurationOutputTypeDef,
-    StepScalingPolicyConfigurationTypeDef,
-    TargetTrackingMetricOutputTypeDef,
-    TargetTrackingMetricTypeDef,
-    DescribeScalingActivitiesResponseTypeDef,
-    DescribeScheduledActionsResponseTypeDef,
-    DescribeScalableTargetsResponseTypeDef,
-    StepScalingPolicyConfigurationUnionTypeDef,
-    TargetTrackingMetricStatOutputTypeDef,
-    TargetTrackingMetricStatTypeDef,
-    TargetTrackingMetricDataQueryOutputTypeDef,
-    TargetTrackingMetricDataQueryTypeDef,
-    CustomizedMetricSpecificationOutputTypeDef,
-    CustomizedMetricSpecificationTypeDef,
-    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-    TargetTrackingScalingPolicyConfigurationTypeDef,
-    ScalingPolicyTypeDef,
-    PutScalingPolicyRequestRequestTypeDef,
-    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
-    DescribeScalingPoliciesResponseTypeDef,
-)
+from types_aiobotocore_application_autoscaling.type_defs import AlarmTypeDef
 
 
 def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/README.md` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-application-autoscaling
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore application-autoscaling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-application-autoscaling"></a>
 
 # types-aiobotocore-application-autoscaling
 
 [![PyPI - types-aiobotocore-application-autoscaling](https://img.shields.io/pypi/v/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-application-autoscaling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-application-autoscaling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/)
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
 [types-aiobotocore-application-autoscaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,104 +305,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_application_autoscaling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApplicationAutoScaling` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/literals/).
+
 ```python
-from types_aiobotocore_application_autoscaling.literals import (
-    AdjustmentTypeType,
-    DescribeScalableTargetsPaginatorName,
-    DescribeScalingActivitiesPaginatorName,
-    DescribeScalingPoliciesPaginatorName,
-    DescribeScheduledActionsPaginatorName,
-    MetricAggregationTypeType,
-    MetricStatisticType,
-    MetricTypeType,
-    PolicyTypeType,
-    ScalableDimensionType,
-    ScalingActivityStatusCodeType,
-    ServiceNamespaceType,
-    ApplicationAutoScalingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_application_autoscaling.literals import AdjustmentTypeType
 
 
 def check_value(value: AdjustmentTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_application_autoscaling.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApplicationAutoScaling` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/type_defs/).
+
 ```python
-from types_aiobotocore_application_autoscaling.type_defs import (
-    AlarmTypeDef,
-    MetricDimensionTypeDef,
-    DeleteScalingPolicyRequestRequestTypeDef,
-    DeleteScheduledActionRequestRequestTypeDef,
-    DeregisterScalableTargetRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeScalableTargetsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeScalingActivitiesRequestRequestTypeDef,
-    DescribeScalingPoliciesRequestRequestTypeDef,
-    DescribeScheduledActionsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NotScaledReasonTypeDef,
-    PredefinedMetricSpecificationTypeDef,
-    ScalableTargetActionTypeDef,
-    TimestampTypeDef,
-    SuspendedStateTypeDef,
-    StepAdjustmentTypeDef,
-    TagResourceRequestRequestTypeDef,
-    TargetTrackingMetricDimensionTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
-    DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
-    DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
-    DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutScalingPolicyResponseTypeDef,
-    RegisterScalableTargetResponseTypeDef,
-    ScalingActivityTypeDef,
-    ScheduledActionTypeDef,
-    PutScheduledActionRequestRequestTypeDef,
-    RegisterScalableTargetRequestRequestTypeDef,
-    ScalableTargetTypeDef,
-    StepScalingPolicyConfigurationOutputTypeDef,
-    StepScalingPolicyConfigurationTypeDef,
-    TargetTrackingMetricOutputTypeDef,
-    TargetTrackingMetricTypeDef,
-    DescribeScalingActivitiesResponseTypeDef,
-    DescribeScheduledActionsResponseTypeDef,
-    DescribeScalableTargetsResponseTypeDef,
-    StepScalingPolicyConfigurationUnionTypeDef,
-    TargetTrackingMetricStatOutputTypeDef,
-    TargetTrackingMetricStatTypeDef,
-    TargetTrackingMetricDataQueryOutputTypeDef,
-    TargetTrackingMetricDataQueryTypeDef,
-    CustomizedMetricSpecificationOutputTypeDef,
-    CustomizedMetricSpecificationTypeDef,
-    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-    TargetTrackingScalingPolicyConfigurationTypeDef,
-    ScalingPolicyTypeDef,
-    PutScalingPolicyRequestRequestTypeDef,
-    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
-    DescribeScalingPoliciesResponseTypeDef,
-)
+from types_aiobotocore_application_autoscaling.type_defs import AlarmTypeDef
 
 
 def get_value() -> AlarmTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/setup.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-autoscaling",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_application_autoscaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__init__.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/__main__.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationAutoScaling 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling\nOther"
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

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
-    StepScalingPolicyConfigurationUnionTypeDef,
+    StepScalingPolicyConfigurationTypeDef,
     SuspendedStateTypeDef,
-    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
+    TargetTrackingScalingPolicyConfigurationTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -250,16 +250,16 @@
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationUnionTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationUnionTypeDef = ...
+        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scaling_policy)
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/client.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     DescribeScalingActivitiesResponseTypeDef,
     DescribeScalingPoliciesResponseTypeDef,
     DescribeScheduledActionsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutScalingPolicyResponseTypeDef,
     RegisterScalableTargetResponseTypeDef,
     ScalableTargetActionTypeDef,
-    StepScalingPolicyConfigurationUnionTypeDef,
+    StepScalingPolicyConfigurationTypeDef,
     SuspendedStateTypeDef,
-    TargetTrackingScalingPolicyConfigurationUnionTypeDef,
+    TargetTrackingScalingPolicyConfigurationTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -234,16 +234,16 @@
         self,
         *,
         PolicyName: str,
         ServiceNamespace: ServiceNamespaceType,
         ResourceId: str,
         ScalableDimension: ScalableDimensionType,
         PolicyType: PolicyTypeType = ...,
-        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationUnionTypeDef = ...,
-        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationUnionTypeDef = ...
+        StepScalingPolicyConfiguration: StepScalingPolicyConfigurationTypeDef = ...,
+        TargetTrackingScalingPolicyConfiguration: TargetTrackingScalingPolicyConfigurationTypeDef = ...
     ) -> PutScalingPolicyResponseTypeDef:
         """
         Creates or updates a scaling policy for an Application Auto Scaling scalable
         target.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#ApplicationAutoScaling.Client.put_scaling_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_autoscaling/client/#put_scaling_policy)
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/literals.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/paginator.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.py` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/type_defs.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -62,33 +61,25 @@
     "PutScalingPolicyResponseTypeDef",
     "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "ScheduledActionTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
-    "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
-    "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
     "DescribeScalableTargetsResponseTypeDef",
-    "StepScalingPolicyConfigurationUnionTypeDef",
-    "TargetTrackingMetricStatOutputTypeDef",
     "TargetTrackingMetricStatTypeDef",
-    "TargetTrackingMetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
-    "CustomizedMetricSpecificationOutputTypeDef",
     "CustomizedMetricSpecificationTypeDef",
-    "TargetTrackingScalingPolicyConfigurationOutputTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
-    "ScalingPolicyTypeDef",
     "PutScalingPolicyRequestRequestTypeDef",
-    "TargetTrackingScalingPolicyConfigurationUnionTypeDef",
+    "ScalingPolicyTypeDef",
     "DescribeScalingPoliciesResponseTypeDef",
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
@@ -156,22 +147,20 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -193,22 +182,20 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeNotScaledActivities": bool,
     },
     total=False,
 )
 
-
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -219,22 +206,20 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -245,22 +230,20 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeScheduledActionsRequestRequestTypeDef(
     _RequiredDescribeScheduledActionsRequestRequestTypeDef,
     _OptionalDescribeScheduledActionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -276,40 +259,36 @@
         "MaxCapacity": int,
         "MinCapacity": int,
         "CurrentCapacity": int,
     },
     total=False,
 )
 
-
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
     pass
 
-
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
-
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
-
 ScalableTargetActionTypeDef = TypedDict(
     "ScalableTargetActionTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
@@ -337,19 +316,17 @@
     {
         "MetricIntervalLowerBound": float,
         "MetricIntervalUpperBound": float,
     },
     total=False,
 )
 
-
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -382,22 +359,20 @@
         "ResourceIds": Sequence[str],
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
     _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
@@ -407,22 +382,20 @@
         "ScalableDimension": ScalableDimensionType,
         "IncludeNotScaledActivities": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
     _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
@@ -432,22 +405,20 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
     _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
@@ -457,22 +428,20 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
     _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -514,19 +483,17 @@
         "StatusMessage": str,
         "Details": str,
         "NotScaledReasons": List[NotScaledReasonTypeDef],
     },
     total=False,
 )
 
-
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
-
 _RequiredScheduledActionTypeDef = TypedDict(
     "_RequiredScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
         "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
         "Schedule": str,
@@ -542,19 +509,17 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-
 class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
-
 _RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
     "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -568,22 +533,20 @@
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
-
 class PutScheduledActionRequestRequestTypeDef(
     _RequiredPutScheduledActionRequestRequestTypeDef,
     _OptionalPutScheduledActionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
@@ -596,22 +559,20 @@
         "RoleARN": str,
         "SuspendedState": SuspendedStateTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RegisterScalableTargetRequestRequestTypeDef(
     _RequiredRegisterScalableTargetRequestRequestTypeDef,
     _OptionalRegisterScalableTargetRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredScalableTargetTypeDef = TypedDict(
     "_RequiredScalableTargetTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -625,57 +586,33 @@
     {
         "SuspendedState": SuspendedStateTypeDef,
         "ScalableTargetARN": str,
     },
     total=False,
 )
 
-
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
-
-StepScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "StepScalingPolicyConfigurationOutputTypeDef",
-    {
-        "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
-        "MinAdjustmentMagnitude": int,
-        "Cooldown": int,
-        "MetricAggregationType": MetricAggregationTypeType,
-    },
-    total=False,
-)
-
 StepScalingPolicyConfigurationTypeDef = TypedDict(
     "StepScalingPolicyConfigurationTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
         "MetricAggregationType": MetricAggregationTypeType,
     },
     total=False,
 )
 
-TargetTrackingMetricOutputTypeDef = TypedDict(
-    "TargetTrackingMetricOutputTypeDef",
-    {
-        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
-        "MetricName": str,
-        "Namespace": str,
-    },
-    total=False,
-)
-
 TargetTrackingMetricTypeDef = TypedDict(
     "TargetTrackingMetricTypeDef",
     {
-        "Dimensions": Sequence[TargetTrackingMetricDimensionTypeDef],
+        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
         "MetricName": str,
         "Namespace": str,
     },
     total=False,
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
@@ -701,39 +638,14 @@
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StepScalingPolicyConfigurationUnionTypeDef = Union[
-    StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
-]
-_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Metric": TargetTrackingMetricOutputTypeDef,
-        "Stat": str,
-    },
-)
-_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Unit": str,
-    },
-    total=False,
-)
-
-
-class TargetTrackingMetricStatOutputTypeDef(
-    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
-):
-    pass
-
-
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
         "Stat": str,
     },
 )
@@ -741,46 +653,19 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
-
-_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Expression": str,
-        "Label": str,
-        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
-        "ReturnData": bool,
-    },
-    total=False,
-)
-
-
-class TargetTrackingMetricDataQueryOutputTypeDef(
-    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
-    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
-):
-    pass
-
-
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalTargetTrackingMetricDataQueryTypeDef = TypedDict(
@@ -790,73 +675,32 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
-
-CustomizedMetricSpecificationOutputTypeDef = TypedDict(
-    "CustomizedMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Statistic": MetricStatisticType,
-        "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
-    },
-    total=False,
-)
-
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
+        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
     },
     total=False,
 )
 
-_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef",
-    {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
-        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
-        "ScaleOutCooldown": int,
-        "ScaleInCooldown": int,
-        "DisableScaleIn": bool,
-    },
-    total=False,
-)
-
-
-class TargetTrackingScalingPolicyConfigurationOutputTypeDef(
-    _RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef,
-    _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
@@ -867,81 +711,69 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
-
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
-
-_RequiredScalingPolicyTypeDef = TypedDict(
-    "_RequiredScalingPolicyTypeDef",
+_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
-        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
-        "PolicyType": PolicyTypeType,
-        "CreationTime": datetime,
     },
 )
-_OptionalScalingPolicyTypeDef = TypedDict(
-    "_OptionalScalingPolicyTypeDef",
+_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyRequestRequestTypeDef",
     {
-        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationOutputTypeDef,
-        "TargetTrackingScalingPolicyConfiguration": (
-            TargetTrackingScalingPolicyConfigurationOutputTypeDef
-        ),
-        "Alarms": List[AlarmTypeDef],
+        "PolicyType": PolicyTypeType,
+        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
+        "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-
-class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
+class PutScalingPolicyRequestRequestTypeDef(
+    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
+):
     pass
 
-
-_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyRequestRequestTypeDef",
+_RequiredScalingPolicyTypeDef = TypedDict(
+    "_RequiredScalingPolicyTypeDef",
     {
+        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
+        "PolicyType": PolicyTypeType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyRequestRequestTypeDef",
+_OptionalScalingPolicyTypeDef = TypedDict(
+    "_OptionalScalingPolicyTypeDef",
     {
-        "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
+        "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-
-class PutScalingPolicyRequestRequestTypeDef(
-    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
-):
+class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-
-TargetTrackingScalingPolicyConfigurationUnionTypeDef = Union[
-    TargetTrackingScalingPolicyConfigurationTypeDef,
-    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-]
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling/type_defs.pyi` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlarmTypeDef",
     "MetricDimensionTypeDef",
     "DeleteScalingPolicyRequestRequestTypeDef",
     "DeleteScheduledActionRequestRequestTypeDef",
     "DeregisterScalableTargetRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -61,33 +62,25 @@
     "PutScalingPolicyResponseTypeDef",
     "RegisterScalableTargetResponseTypeDef",
     "ScalingActivityTypeDef",
     "ScheduledActionTypeDef",
     "PutScheduledActionRequestRequestTypeDef",
     "RegisterScalableTargetRequestRequestTypeDef",
     "ScalableTargetTypeDef",
-    "StepScalingPolicyConfigurationOutputTypeDef",
     "StepScalingPolicyConfigurationTypeDef",
-    "TargetTrackingMetricOutputTypeDef",
     "TargetTrackingMetricTypeDef",
     "DescribeScalingActivitiesResponseTypeDef",
     "DescribeScheduledActionsResponseTypeDef",
     "DescribeScalableTargetsResponseTypeDef",
-    "StepScalingPolicyConfigurationUnionTypeDef",
-    "TargetTrackingMetricStatOutputTypeDef",
     "TargetTrackingMetricStatTypeDef",
-    "TargetTrackingMetricDataQueryOutputTypeDef",
     "TargetTrackingMetricDataQueryTypeDef",
-    "CustomizedMetricSpecificationOutputTypeDef",
     "CustomizedMetricSpecificationTypeDef",
-    "TargetTrackingScalingPolicyConfigurationOutputTypeDef",
     "TargetTrackingScalingPolicyConfigurationTypeDef",
-    "ScalingPolicyTypeDef",
     "PutScalingPolicyRequestRequestTypeDef",
-    "TargetTrackingScalingPolicyConfigurationUnionTypeDef",
+    "ScalingPolicyTypeDef",
     "DescribeScalingPoliciesResponseTypeDef",
 )
 
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "AlarmName": str,
@@ -155,20 +148,22 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalableTargetsRequestRequestTypeDef(
     _RequiredDescribeScalableTargetsRequestRequestTypeDef,
     _OptionalDescribeScalableTargetsRequestRequestTypeDef,
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -190,20 +185,22 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeNotScaledActivities": bool,
     },
     total=False,
 )
 
+
 class DescribeScalingActivitiesRequestRequestTypeDef(
     _RequiredDescribeScalingActivitiesRequestRequestTypeDef,
     _OptionalDescribeScalingActivitiesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestRequestTypeDef = TypedDict(
@@ -214,20 +211,22 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScalingPoliciesRequestRequestTypeDef(
     _RequiredDescribeScalingPoliciesRequestRequestTypeDef,
     _OptionalDescribeScalingPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestRequestTypeDef = TypedDict(
@@ -238,20 +237,22 @@
         "ScalableDimension": ScalableDimensionType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeScheduledActionsRequestRequestTypeDef(
     _RequiredDescribeScheduledActionsRequestRequestTypeDef,
     _OptionalDescribeScheduledActionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
@@ -267,36 +268,40 @@
         "MaxCapacity": int,
         "MinCapacity": int,
         "CurrentCapacity": int,
     },
     total=False,
 )
 
+
 class NotScaledReasonTypeDef(_RequiredNotScaledReasonTypeDef, _OptionalNotScaledReasonTypeDef):
     pass
 
+
 _RequiredPredefinedMetricSpecificationTypeDef = TypedDict(
     "_RequiredPredefinedMetricSpecificationTypeDef",
     {
         "PredefinedMetricType": MetricTypeType,
     },
 )
 _OptionalPredefinedMetricSpecificationTypeDef = TypedDict(
     "_OptionalPredefinedMetricSpecificationTypeDef",
     {
         "ResourceLabel": str,
     },
     total=False,
 )
 
+
 class PredefinedMetricSpecificationTypeDef(
     _RequiredPredefinedMetricSpecificationTypeDef, _OptionalPredefinedMetricSpecificationTypeDef
 ):
     pass
 
+
 ScalableTargetActionTypeDef = TypedDict(
     "ScalableTargetActionTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
     total=False,
@@ -324,17 +329,19 @@
     {
         "MetricIntervalLowerBound": float,
         "MetricIntervalUpperBound": float,
     },
     total=False,
 )
 
+
 class StepAdjustmentTypeDef(_RequiredStepAdjustmentTypeDef, _OptionalStepAdjustmentTypeDef):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -367,20 +374,22 @@
         "ResourceIds": Sequence[str],
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef(
     _RequiredDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
     _OptionalDescribeScalableTargetsRequestDescribeScalableTargetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef = TypedDict(
@@ -390,20 +399,22 @@
         "ScalableDimension": ScalableDimensionType,
         "IncludeNotScaledActivities": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef(
     _RequiredDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
     _OptionalDescribeScalingActivitiesRequestDescribeScalingActivitiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
     "_RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef = TypedDict(
@@ -413,20 +424,22 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef(
     _RequiredDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
     _OptionalDescribeScalingPoliciesRequestDescribeScalingPoliciesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
     "_RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
     },
 )
 _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef = TypedDict(
@@ -436,20 +449,22 @@
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef(
     _RequiredDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
     _OptionalDescribeScheduledActionsRequestDescribeScheduledActionsPaginateTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -491,17 +506,19 @@
         "StatusMessage": str,
         "Details": str,
         "NotScaledReasons": List[NotScaledReasonTypeDef],
     },
     total=False,
 )
 
+
 class ScalingActivityTypeDef(_RequiredScalingActivityTypeDef, _OptionalScalingActivityTypeDef):
     pass
 
+
 _RequiredScheduledActionTypeDef = TypedDict(
     "_RequiredScheduledActionTypeDef",
     {
         "ScheduledActionName": str,
         "ScheduledActionARN": str,
         "ServiceNamespace": ServiceNamespaceType,
         "Schedule": str,
@@ -517,17 +534,19 @@
         "StartTime": datetime,
         "EndTime": datetime,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
+
 class ScheduledActionTypeDef(_RequiredScheduledActionTypeDef, _OptionalScheduledActionTypeDef):
     pass
 
+
 _RequiredPutScheduledActionRequestRequestTypeDef = TypedDict(
     "_RequiredPutScheduledActionRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ScheduledActionName": str,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
@@ -541,20 +560,22 @@
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
         "ScalableTargetAction": ScalableTargetActionTypeDef,
     },
     total=False,
 )
 
+
 class PutScheduledActionRequestRequestTypeDef(
     _RequiredPutScheduledActionRequestRequestTypeDef,
     _OptionalPutScheduledActionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredRegisterScalableTargetRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterScalableTargetRequestRequestTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
     },
@@ -567,20 +588,22 @@
         "RoleARN": str,
         "SuspendedState": SuspendedStateTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RegisterScalableTargetRequestRequestTypeDef(
     _RequiredRegisterScalableTargetRequestRequestTypeDef,
     _OptionalRegisterScalableTargetRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredScalableTargetTypeDef = TypedDict(
     "_RequiredScalableTargetTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
@@ -594,55 +617,35 @@
     {
         "SuspendedState": SuspendedStateTypeDef,
         "ScalableTargetARN": str,
     },
     total=False,
 )
 
+
 class ScalableTargetTypeDef(_RequiredScalableTargetTypeDef, _OptionalScalableTargetTypeDef):
     pass
 
-StepScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "StepScalingPolicyConfigurationOutputTypeDef",
-    {
-        "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": List[StepAdjustmentTypeDef],
-        "MinAdjustmentMagnitude": int,
-        "Cooldown": int,
-        "MetricAggregationType": MetricAggregationTypeType,
-    },
-    total=False,
-)
 
 StepScalingPolicyConfigurationTypeDef = TypedDict(
     "StepScalingPolicyConfigurationTypeDef",
     {
         "AdjustmentType": AdjustmentTypeType,
-        "StepAdjustments": Sequence[StepAdjustmentTypeDef],
+        "StepAdjustments": List[StepAdjustmentTypeDef],
         "MinAdjustmentMagnitude": int,
         "Cooldown": int,
         "MetricAggregationType": MetricAggregationTypeType,
     },
     total=False,
 )
 
-TargetTrackingMetricOutputTypeDef = TypedDict(
-    "TargetTrackingMetricOutputTypeDef",
-    {
-        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
-        "MetricName": str,
-        "Namespace": str,
-    },
-    total=False,
-)
-
 TargetTrackingMetricTypeDef = TypedDict(
     "TargetTrackingMetricTypeDef",
     {
-        "Dimensions": Sequence[TargetTrackingMetricDimensionTypeDef],
+        "Dimensions": List[TargetTrackingMetricDimensionTypeDef],
         "MetricName": str,
         "Namespace": str,
     },
     total=False,
 )
 
 DescribeScalingActivitiesResponseTypeDef = TypedDict(
@@ -668,37 +671,14 @@
     {
         "ScalableTargets": List[ScalableTargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StepScalingPolicyConfigurationUnionTypeDef = Union[
-    StepScalingPolicyConfigurationTypeDef, StepScalingPolicyConfigurationOutputTypeDef
-]
-_RequiredTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Metric": TargetTrackingMetricOutputTypeDef,
-        "Stat": str,
-    },
-)
-_OptionalTargetTrackingMetricStatOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricStatOutputTypeDef",
-    {
-        "Unit": str,
-    },
-    total=False,
-)
-
-class TargetTrackingMetricStatOutputTypeDef(
-    _RequiredTargetTrackingMetricStatOutputTypeDef, _OptionalTargetTrackingMetricStatOutputTypeDef
-):
-    pass
-
 _RequiredTargetTrackingMetricStatTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricStatTypeDef",
     {
         "Metric": TargetTrackingMetricTypeDef,
         "Stat": str,
     },
 )
@@ -706,41 +686,20 @@
     "_OptionalTargetTrackingMetricStatTypeDef",
     {
         "Unit": str,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricStatTypeDef(
     _RequiredTargetTrackingMetricStatTypeDef, _OptionalTargetTrackingMetricStatTypeDef
 ):
     pass
 
-_RequiredTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalTargetTrackingMetricDataQueryOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingMetricDataQueryOutputTypeDef",
-    {
-        "Expression": str,
-        "Label": str,
-        "MetricStat": TargetTrackingMetricStatOutputTypeDef,
-        "ReturnData": bool,
-    },
-    total=False,
-)
-
-class TargetTrackingMetricDataQueryOutputTypeDef(
-    _RequiredTargetTrackingMetricDataQueryOutputTypeDef,
-    _OptionalTargetTrackingMetricDataQueryOutputTypeDef,
-):
-    pass
 
 _RequiredTargetTrackingMetricDataQueryTypeDef = TypedDict(
     "_RequiredTargetTrackingMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
@@ -751,69 +710,34 @@
         "Label": str,
         "MetricStat": TargetTrackingMetricStatTypeDef,
         "ReturnData": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingMetricDataQueryTypeDef(
     _RequiredTargetTrackingMetricDataQueryTypeDef, _OptionalTargetTrackingMetricDataQueryTypeDef
 ):
     pass
 
-CustomizedMetricSpecificationOutputTypeDef = TypedDict(
-    "CustomizedMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Statistic": MetricStatisticType,
-        "Unit": str,
-        "Metrics": List[TargetTrackingMetricDataQueryOutputTypeDef],
-    },
-    total=False,
-)
 
 CustomizedMetricSpecificationTypeDef = TypedDict(
     "CustomizedMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
-        "Dimensions": Sequence[MetricDimensionTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
         "Statistic": MetricStatisticType,
         "Unit": str,
-        "Metrics": Sequence[TargetTrackingMetricDataQueryTypeDef],
-    },
-    total=False,
-)
-
-_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef",
-    {
-        "TargetValue": float,
-    },
-)
-_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef",
-    {
-        "PredefinedMetricSpecification": PredefinedMetricSpecificationTypeDef,
-        "CustomizedMetricSpecification": CustomizedMetricSpecificationOutputTypeDef,
-        "ScaleOutCooldown": int,
-        "ScaleInCooldown": int,
-        "DisableScaleIn": bool,
+        "Metrics": List[TargetTrackingMetricDataQueryTypeDef],
     },
     total=False,
 )
 
-class TargetTrackingScalingPolicyConfigurationOutputTypeDef(
-    _RequiredTargetTrackingScalingPolicyConfigurationOutputTypeDef,
-    _OptionalTargetTrackingScalingPolicyConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingScalingPolicyConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingScalingPolicyConfigurationTypeDef = TypedDict(
@@ -824,75 +748,75 @@
         "ScaleOutCooldown": int,
         "ScaleInCooldown": int,
         "DisableScaleIn": bool,
     },
     total=False,
 )
 
+
 class TargetTrackingScalingPolicyConfigurationTypeDef(
     _RequiredTargetTrackingScalingPolicyConfigurationTypeDef,
     _OptionalTargetTrackingScalingPolicyConfigurationTypeDef,
 ):
     pass
 
-_RequiredScalingPolicyTypeDef = TypedDict(
-    "_RequiredScalingPolicyTypeDef",
+
+_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredPutScalingPolicyRequestRequestTypeDef",
     {
-        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
-        "PolicyType": PolicyTypeType,
-        "CreationTime": datetime,
     },
 )
-_OptionalScalingPolicyTypeDef = TypedDict(
-    "_OptionalScalingPolicyTypeDef",
+_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalPutScalingPolicyRequestRequestTypeDef",
     {
-        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationOutputTypeDef,
-        "TargetTrackingScalingPolicyConfiguration": (
-            TargetTrackingScalingPolicyConfigurationOutputTypeDef
-        ),
-        "Alarms": List[AlarmTypeDef],
+        "PolicyType": PolicyTypeType,
+        "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
+        "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
     },
     total=False,
 )
 
-class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
+
+class PutScalingPolicyRequestRequestTypeDef(
+    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
+):
     pass
 
-_RequiredPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredPutScalingPolicyRequestRequestTypeDef",
+
+_RequiredScalingPolicyTypeDef = TypedDict(
+    "_RequiredScalingPolicyTypeDef",
     {
+        "PolicyARN": str,
         "PolicyName": str,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
+        "PolicyType": PolicyTypeType,
+        "CreationTime": datetime,
     },
 )
-_OptionalPutScalingPolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalPutScalingPolicyRequestRequestTypeDef",
+_OptionalScalingPolicyTypeDef = TypedDict(
+    "_OptionalScalingPolicyTypeDef",
     {
-        "PolicyType": PolicyTypeType,
         "StepScalingPolicyConfiguration": StepScalingPolicyConfigurationTypeDef,
         "TargetTrackingScalingPolicyConfiguration": TargetTrackingScalingPolicyConfigurationTypeDef,
+        "Alarms": List[AlarmTypeDef],
     },
     total=False,
 )
 
-class PutScalingPolicyRequestRequestTypeDef(
-    _RequiredPutScalingPolicyRequestRequestTypeDef, _OptionalPutScalingPolicyRequestRequestTypeDef
-):
+
+class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-TargetTrackingScalingPolicyConfigurationUnionTypeDef = Union[
-    TargetTrackingScalingPolicyConfigurationTypeDef,
-    TargetTrackingScalingPolicyConfigurationOutputTypeDef,
-]
+
 DescribeScalingPoliciesResponseTypeDef = TypedDict(
     "DescribeScalingPoliciesResponseTypeDef",
     {
         "ScalingPolicies": List[ScalingPolicyTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-application-autoscaling-2.5.2.post1/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt` & `types-aiobotocore-application-autoscaling-2.5.2.post2/types_aiobotocore_application_autoscaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

