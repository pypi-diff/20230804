# Comparing `tmp/types-aiobotocore-autoscaling-plans-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-autoscaling-plans-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-autoscaling-plans-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1.tar` & `types-aiobotocore-autoscaling-plans-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13860 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-08-02 14:33:41.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-08-02 14:33:41.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:40.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.185648 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:51:55.000000 types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.247223 types-aiobotocore-autoscaling-plans-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-04 12:00:28.247223 types-aiobotocore-autoscaling-plans-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.247223 types-aiobotocore-autoscaling-plans-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.243223 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14086 2023-08-04 11:40:52.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14061 2023-08-04 11:40:52.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:51.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.247223 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:28.000000 types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/LICENSE` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-autoscaling-plans
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,91 +297,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_autoscaling_plans.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `AutoScalingPlans` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/literals/).
+
 ```python
-from types_aiobotocore_autoscaling_plans.literals import (
-    DescribeScalingPlanResourcesPaginatorName,
-    DescribeScalingPlansPaginatorName,
-    ForecastDataTypeType,
-    LoadMetricTypeType,
-    MetricStatisticType,
-    PolicyTypeType,
-    PredictiveScalingMaxCapacityBehaviorType,
-    PredictiveScalingModeType,
-    ScalableDimensionType,
-    ScalingMetricTypeType,
-    ScalingPlanStatusCodeType,
-    ScalingPolicyUpdateBehaviorType,
-    ScalingStatusCodeType,
-    ServiceNamespaceType,
-    AutoScalingPlansServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_autoscaling_plans.literals import DescribeScalingPlanResourcesPaginatorName
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_autoscaling_plans.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AutoScalingPlans` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/).
+
 ```python
-from types_aiobotocore_autoscaling_plans.type_defs import (
-    TagFilterOutputTypeDef,
-    TagFilterTypeDef,
-    ResponseMetadataTypeDef,
-    MetricDimensionTypeDef,
-    DatapointTypeDef,
-    DeleteScalingPlanRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeScalingPlanResourcesRequestRequestTypeDef,
-    TimestampTypeDef,
-    PredefinedLoadMetricSpecificationTypeDef,
-    PredefinedScalingMetricSpecificationTypeDef,
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
-    CreateScalingPlanResponseTypeDef,
-    CustomizedLoadMetricSpecificationOutputTypeDef,
-    CustomizedLoadMetricSpecificationTypeDef,
-    CustomizedScalingMetricSpecificationOutputTypeDef,
-    CustomizedScalingMetricSpecificationTypeDef,
-    GetScalingPlanResourceForecastDataResponseTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
-    ApplicationSourceUnionTypeDef,
-    TargetTrackingConfigurationOutputTypeDef,
-    TargetTrackingConfigurationTypeDef,
-    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
-    DescribeScalingPlansRequestRequestTypeDef,
-    ScalingInstructionOutputTypeDef,
-    ScalingPolicyTypeDef,
-    ScalingInstructionTypeDef,
-    ScalingPlanTypeDef,
-    ScalingPlanResourceTypeDef,
-    ScalingInstructionUnionTypeDef,
-    DescribeScalingPlansResponseTypeDef,
-    DescribeScalingPlanResourcesResponseTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
-)
+from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
 
 
-def get_value() -> TagFilterOutputTypeDef:
+def get_value() -> TagFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/README.md` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-autoscaling-plans
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore autoscaling-plans type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,91 +297,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_autoscaling_plans.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `AutoScalingPlans` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/literals/).
+
 ```python
-from types_aiobotocore_autoscaling_plans.literals import (
-    DescribeScalingPlanResourcesPaginatorName,
-    DescribeScalingPlansPaginatorName,
-    ForecastDataTypeType,
-    LoadMetricTypeType,
-    MetricStatisticType,
-    PolicyTypeType,
-    PredictiveScalingMaxCapacityBehaviorType,
-    PredictiveScalingModeType,
-    ScalableDimensionType,
-    ScalingMetricTypeType,
-    ScalingPlanStatusCodeType,
-    ScalingPolicyUpdateBehaviorType,
-    ScalingStatusCodeType,
-    ServiceNamespaceType,
-    AutoScalingPlansServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_autoscaling_plans.literals import DescribeScalingPlanResourcesPaginatorName
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_autoscaling_plans.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AutoScalingPlans` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/).
+
 ```python
-from types_aiobotocore_autoscaling_plans.type_defs import (
-    TagFilterOutputTypeDef,
-    TagFilterTypeDef,
-    ResponseMetadataTypeDef,
-    MetricDimensionTypeDef,
-    DatapointTypeDef,
-    DeleteScalingPlanRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeScalingPlanResourcesRequestRequestTypeDef,
-    TimestampTypeDef,
-    PredefinedLoadMetricSpecificationTypeDef,
-    PredefinedScalingMetricSpecificationTypeDef,
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
-    CreateScalingPlanResponseTypeDef,
-    CustomizedLoadMetricSpecificationOutputTypeDef,
-    CustomizedLoadMetricSpecificationTypeDef,
-    CustomizedScalingMetricSpecificationOutputTypeDef,
-    CustomizedScalingMetricSpecificationTypeDef,
-    GetScalingPlanResourceForecastDataResponseTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
-    ApplicationSourceUnionTypeDef,
-    TargetTrackingConfigurationOutputTypeDef,
-    TargetTrackingConfigurationTypeDef,
-    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
-    DescribeScalingPlansRequestRequestTypeDef,
-    ScalingInstructionOutputTypeDef,
-    ScalingPolicyTypeDef,
-    ScalingInstructionTypeDef,
-    ScalingPlanTypeDef,
-    ScalingPlanResourceTypeDef,
-    ScalingInstructionUnionTypeDef,
-    DescribeScalingPlansResponseTypeDef,
-    DescribeScalingPlanResourcesResponseTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
-)
+from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
 
 
-def get_value() -> TagFilterOutputTypeDef:
+def get_value() -> TagFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/setup.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-autoscaling-plans",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_autoscaling_plans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__init__.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/__main__.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AutoScalingPlans 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans\nOther"
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

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
-    ApplicationSourceUnionTypeDef,
+    ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    ScalingInstructionUnionTypeDef,
+    ScalingInstructionTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -92,16 +92,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#close)
         """
 
     async def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: ApplicationSourceUnionTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef]
+        ApplicationSource: ApplicationSourceTypeDef,
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -132,15 +132,15 @@
         """
 
     async def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
+        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -181,16 +181,16 @@
         """
 
     async def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: ApplicationSourceUnionTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef] = ...
+        ApplicationSource: ApplicationSourceTypeDef = ...,
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/client.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ForecastDataTypeType, ScalableDimensionType, ServiceNamespaceType
 from .paginator import DescribeScalingPlanResourcesPaginator, DescribeScalingPlansPaginator
 from .type_defs import (
-    ApplicationSourceUnionTypeDef,
+    ApplicationSourceTypeDef,
     CreateScalingPlanResponseTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     GetScalingPlanResourceForecastDataResponseTypeDef,
-    ScalingInstructionUnionTypeDef,
+    ScalingInstructionTypeDef,
     TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -85,16 +85,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#close)
         """
     async def create_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
-        ApplicationSource: ApplicationSourceUnionTypeDef,
-        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef]
+        ApplicationSource: ApplicationSourceTypeDef,
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef]
     ) -> CreateScalingPlanResponseTypeDef:
         """
         Creates a scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.create_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#create_scaling_plan)
         """
@@ -122,15 +122,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#describe_scaling_plan_resources)
         """
     async def describe_scaling_plans(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
+        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> DescribeScalingPlansResponseTypeDef:
         """
         Describes one or more of your scaling plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.describe_scaling_plans)
@@ -168,16 +168,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#get_scaling_plan_resource_forecast_data)
         """
     async def update_scaling_plan(
         self,
         *,
         ScalingPlanName: str,
         ScalingPlanVersion: int,
-        ApplicationSource: ApplicationSourceUnionTypeDef = ...,
-        ScalingInstructions: Sequence[ScalingInstructionUnionTypeDef] = ...
+        ApplicationSource: ApplicationSourceTypeDef = ...,
+        ScalingInstructions: Sequence[ScalingInstructionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Updates the specified scaling plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Client.update_scaling_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/client/#update_scaling_plan)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/literals.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
-    ApplicationSourceUnionTypeDef,
+    ApplicationSourceTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
@@ -73,14 +73,14 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
+        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/paginator.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 """
 from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import (
-    ApplicationSourceUnionTypeDef,
+    ApplicationSourceTypeDef,
     DescribeScalingPlanResourcesResponseTypeDef,
     DescribeScalingPlansResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeScalingPlanResourcesPaginator", "DescribeScalingPlansPaginator")
 
@@ -69,14 +69,14 @@
     """
 
     def paginate(
         self,
         *,
         ScalingPlanNames: Sequence[str] = ...,
         ScalingPlanVersion: int = ...,
-        ApplicationSources: Sequence[ApplicationSourceUnionTypeDef] = ...,
+        ApplicationSources: Sequence[ApplicationSourceTypeDef] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeScalingPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#AutoScalingPlans.Paginator.DescribeScalingPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/paginators/#describescalingplanspaginator)
         """
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.py` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling-plans service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterOutputTypeDef
+    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
 
-    data: TagFilterOutputTypeDef = ...
+    data: TagFilterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -36,59 +36,42 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
     "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "TimestampTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
-    "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
     "CreateScalingPlanResponseTypeDef",
-    "CustomizedLoadMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
-    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    "ApplicationSourceUnionTypeDef",
-    "TargetTrackingConfigurationOutputTypeDef",
-    "TargetTrackingConfigurationTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
-    "ScalingInstructionOutputTypeDef",
-    "ScalingPolicyTypeDef",
+    "TargetTrackingConfigurationTypeDef",
     "ScalingInstructionTypeDef",
+    "ScalingPolicyTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
     "ScalingPlanTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
     "ScalingPlanResourceTypeDef",
-    "ScalingInstructionUnionTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
-)
-
-TagFilterOutputTypeDef = TypedDict(
-    "TagFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-    total=False,
 )
 
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -207,23 +190,14 @@
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
 
-ApplicationSourceOutputTypeDef = TypedDict(
-    "ApplicationSourceOutputTypeDef",
-    {
-        "CloudFormationStackARN": str,
-        "TagFilters": List[TagFilterOutputTypeDef],
-    },
-    total=False,
-)
-
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
@@ -233,39 +207,14 @@
     "CreateScalingPlanResponseTypeDef",
     {
         "ScalingPlanVersion": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": MetricStatisticType,
-    },
-)
-_OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Unit": str,
-    },
-    total=False,
-)
-
-
-class CustomizedLoadMetricSpecificationOutputTypeDef(
-    _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
-    _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -283,39 +232,14 @@
 class CustomizedLoadMetricSpecificationTypeDef(
     _RequiredCustomizedLoadMetricSpecificationTypeDef,
     _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
 
-_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": MetricStatisticType,
-    },
-)
-_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Unit": str,
-    },
-    total=False,
-)
-
-
-class CustomizedScalingMetricSpecificationOutputTypeDef(
-    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
-    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -378,42 +302,37 @@
         "ScalableDimension": ScalableDimensionType,
         "ForecastDataType": ForecastDataTypeType,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
 
-ApplicationSourceUnionTypeDef = Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
-        "TargetValue": float,
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+
+DescribeScalingPlansRequestRequestTypeDef = TypedDict(
+    "DescribeScalingPlansRequestRequestTypeDef",
     {
-        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationTypeDef,
-        "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
-        "DisableScaleIn": bool,
-        "ScaleOutCooldown": int,
-        "ScaleInCooldown": int,
-        "EstimatedInstanceWarmup": int,
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-
-class TargetTrackingConfigurationOutputTypeDef(
-    _RequiredTargetTrackingConfigurationOutputTypeDef,
-    _OptionalTargetTrackingConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -432,130 +351,83 @@
 
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
 
-DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
-    {
-        "ScalingPlanNames": Sequence[str],
-        "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScalingPlansRequestRequestTypeDef = TypedDict(
-    "DescribeScalingPlansRequestRequestTypeDef",
-    {
-        "ScalingPlanNames": Sequence[str],
-        "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-_RequiredScalingInstructionOutputTypeDef = TypedDict(
-    "_RequiredScalingInstructionOutputTypeDef",
+_RequiredScalingInstructionTypeDef = TypedDict(
+    "_RequiredScalingInstructionTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
         "MaxCapacity": int,
-        "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
+        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
     },
 )
-_OptionalScalingInstructionOutputTypeDef = TypedDict(
-    "_OptionalScalingInstructionOutputTypeDef",
+_OptionalScalingInstructionTypeDef = TypedDict(
+    "_OptionalScalingInstructionTypeDef",
     {
         "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
     },
     total=False,
 )
 
 
-class ScalingInstructionOutputTypeDef(
-    _RequiredScalingInstructionOutputTypeDef, _OptionalScalingInstructionOutputTypeDef
+class ScalingInstructionTypeDef(
+    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
 ):
     pass
 
 
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyType": Literal["TargetTrackingScaling"],
     },
 )
 _OptionalScalingPolicyTypeDef = TypedDict(
     "_OptionalScalingPolicyTypeDef",
     {
-        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
 
-_RequiredScalingInstructionTypeDef = TypedDict(
-    "_RequiredScalingInstructionTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "MinCapacity": int,
-        "MaxCapacity": int,
-        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
-    },
-)
-_OptionalScalingInstructionTypeDef = TypedDict(
-    "_OptionalScalingInstructionTypeDef",
+CreateScalingPlanRequestRequestTypeDef = TypedDict(
+    "CreateScalingPlanRequestRequestTypeDef",
     {
-        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
-        "ScheduledActionBufferTime": int,
-        "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
-        "PredictiveScalingMaxCapacityBuffer": int,
-        "PredictiveScalingMode": PredictiveScalingModeType,
-        "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
-        "DisableDynamicScaling": bool,
+        "ScalingPlanName": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
     },
-    total=False,
 )
 
-
-class ScalingInstructionTypeDef(
-    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
-):
-    pass
-
-
 _RequiredScalingPlanTypeDef = TypedDict(
     "_RequiredScalingPlanTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSource": ApplicationSourceOutputTypeDef,
-        "ScalingInstructions": List[ScalingInstructionOutputTypeDef],
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": List[ScalingInstructionTypeDef],
         "StatusCode": ScalingPlanStatusCodeType,
     },
 )
 _OptionalScalingPlanTypeDef = TypedDict(
     "_OptionalScalingPlanTypeDef",
     {
         "StatusMessage": str,
@@ -566,14 +438,37 @@
 )
 
 
 class ScalingPlanTypeDef(_RequiredScalingPlanTypeDef, _OptionalScalingPlanTypeDef):
     pass
 
 
+_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateScalingPlanRequestRequestTypeDef(
+    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredScalingPlanResourceTypeDef = TypedDict(
     "_RequiredScalingPlanResourceTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -593,15 +488,14 @@
 
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
 
-ScalingInstructionUnionTypeDef = Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -611,38 +505,7 @@
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateScalingPlanRequestRequestTypeDef = TypedDict(
-    "CreateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
-    },
-)
-
-_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateScalingPlanRequestRequestTypeDef(
-    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans/type_defs.pyi` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for autoscaling-plans service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterOutputTypeDef
+    from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
 
-    data: TagFilterOutputTypeDef = ...
+    data: TagFilterTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,59 +35,42 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "TagFilterOutputTypeDef",
     "TagFilterTypeDef",
     "ResponseMetadataTypeDef",
     "MetricDimensionTypeDef",
     "DatapointTypeDef",
     "DeleteScalingPlanRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeScalingPlanResourcesRequestRequestTypeDef",
     "TimestampTypeDef",
     "PredefinedLoadMetricSpecificationTypeDef",
     "PredefinedScalingMetricSpecificationTypeDef",
-    "ApplicationSourceOutputTypeDef",
     "ApplicationSourceTypeDef",
     "CreateScalingPlanResponseTypeDef",
-    "CustomizedLoadMetricSpecificationOutputTypeDef",
     "CustomizedLoadMetricSpecificationTypeDef",
-    "CustomizedScalingMetricSpecificationOutputTypeDef",
     "CustomizedScalingMetricSpecificationTypeDef",
     "GetScalingPlanResourceForecastDataResponseTypeDef",
     "DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef",
     "GetScalingPlanResourceForecastDataRequestRequestTypeDef",
-    "ApplicationSourceUnionTypeDef",
-    "TargetTrackingConfigurationOutputTypeDef",
-    "TargetTrackingConfigurationTypeDef",
     "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     "DescribeScalingPlansRequestRequestTypeDef",
-    "ScalingInstructionOutputTypeDef",
-    "ScalingPolicyTypeDef",
+    "TargetTrackingConfigurationTypeDef",
     "ScalingInstructionTypeDef",
+    "ScalingPolicyTypeDef",
+    "CreateScalingPlanRequestRequestTypeDef",
     "ScalingPlanTypeDef",
+    "UpdateScalingPlanRequestRequestTypeDef",
     "ScalingPlanResourceTypeDef",
-    "ScalingInstructionUnionTypeDef",
     "DescribeScalingPlansResponseTypeDef",
     "DescribeScalingPlanResourcesResponseTypeDef",
-    "CreateScalingPlanRequestRequestTypeDef",
-    "UpdateScalingPlanRequestRequestTypeDef",
-)
-
-TagFilterOutputTypeDef = TypedDict(
-    "TagFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-    total=False,
 )
 
 TagFilterTypeDef = TypedDict(
     "TagFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
@@ -200,23 +183,14 @@
 
 class PredefinedScalingMetricSpecificationTypeDef(
     _RequiredPredefinedScalingMetricSpecificationTypeDef,
     _OptionalPredefinedScalingMetricSpecificationTypeDef,
 ):
     pass
 
-ApplicationSourceOutputTypeDef = TypedDict(
-    "ApplicationSourceOutputTypeDef",
-    {
-        "CloudFormationStackARN": str,
-        "TagFilters": List[TagFilterOutputTypeDef],
-    },
-    total=False,
-)
-
 ApplicationSourceTypeDef = TypedDict(
     "ApplicationSourceTypeDef",
     {
         "CloudFormationStackARN": str,
         "TagFilters": Sequence[TagFilterTypeDef],
     },
     total=False,
@@ -226,37 +200,14 @@
     "CreateScalingPlanResponseTypeDef",
     {
         "ScalingPlanVersion": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredCustomizedLoadMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": MetricStatisticType,
-    },
-)
-_OptionalCustomizedLoadMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalCustomizedLoadMetricSpecificationOutputTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Unit": str,
-    },
-    total=False,
-)
-
-class CustomizedLoadMetricSpecificationOutputTypeDef(
-    _RequiredCustomizedLoadMetricSpecificationOutputTypeDef,
-    _OptionalCustomizedLoadMetricSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredCustomizedLoadMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedLoadMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -272,37 +223,14 @@
 
 class CustomizedLoadMetricSpecificationTypeDef(
     _RequiredCustomizedLoadMetricSpecificationTypeDef,
     _OptionalCustomizedLoadMetricSpecificationTypeDef,
 ):
     pass
 
-_RequiredCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_RequiredCustomizedScalingMetricSpecificationOutputTypeDef",
-    {
-        "MetricName": str,
-        "Namespace": str,
-        "Statistic": MetricStatisticType,
-    },
-)
-_OptionalCustomizedScalingMetricSpecificationOutputTypeDef = TypedDict(
-    "_OptionalCustomizedScalingMetricSpecificationOutputTypeDef",
-    {
-        "Dimensions": List[MetricDimensionTypeDef],
-        "Unit": str,
-    },
-    total=False,
-)
-
-class CustomizedScalingMetricSpecificationOutputTypeDef(
-    _RequiredCustomizedScalingMetricSpecificationOutputTypeDef,
-    _OptionalCustomizedScalingMetricSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredCustomizedScalingMetricSpecificationTypeDef = TypedDict(
     "_RequiredCustomizedScalingMetricSpecificationTypeDef",
     {
         "MetricName": str,
         "Namespace": str,
         "Statistic": MetricStatisticType,
     },
@@ -361,40 +289,37 @@
         "ScalableDimension": ScalableDimensionType,
         "ForecastDataType": ForecastDataTypeType,
         "StartTime": TimestampTypeDef,
         "EndTime": TimestampTypeDef,
     },
 )
 
-ApplicationSourceUnionTypeDef = Union[ApplicationSourceTypeDef, ApplicationSourceOutputTypeDef]
-_RequiredTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredTargetTrackingConfigurationOutputTypeDef",
+DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
+    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
     {
-        "TargetValue": float,
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalTargetTrackingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalTargetTrackingConfigurationOutputTypeDef",
+
+DescribeScalingPlansRequestRequestTypeDef = TypedDict(
+    "DescribeScalingPlansRequestRequestTypeDef",
     {
-        "PredefinedScalingMetricSpecification": PredefinedScalingMetricSpecificationTypeDef,
-        "CustomizedScalingMetricSpecification": CustomizedScalingMetricSpecificationOutputTypeDef,
-        "DisableScaleIn": bool,
-        "ScaleOutCooldown": int,
-        "ScaleInCooldown": int,
-        "EstimatedInstanceWarmup": int,
+        "ScalingPlanNames": Sequence[str],
+        "ScalingPlanVersion": int,
+        "ApplicationSources": Sequence[ApplicationSourceTypeDef],
+        "MaxResults": int,
+        "NextToken": str,
     },
     total=False,
 )
 
-class TargetTrackingConfigurationOutputTypeDef(
-    _RequiredTargetTrackingConfigurationOutputTypeDef,
-    _OptionalTargetTrackingConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredTargetTrackingConfigurationTypeDef = TypedDict(
     "_RequiredTargetTrackingConfigurationTypeDef",
     {
         "TargetValue": float,
     },
 )
 _OptionalTargetTrackingConfigurationTypeDef = TypedDict(
@@ -411,124 +336,79 @@
 )
 
 class TargetTrackingConfigurationTypeDef(
     _RequiredTargetTrackingConfigurationTypeDef, _OptionalTargetTrackingConfigurationTypeDef
 ):
     pass
 
-DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef = TypedDict(
-    "DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef",
-    {
-        "ScalingPlanNames": Sequence[str],
-        "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-DescribeScalingPlansRequestRequestTypeDef = TypedDict(
-    "DescribeScalingPlansRequestRequestTypeDef",
-    {
-        "ScalingPlanNames": Sequence[str],
-        "ScalingPlanVersion": int,
-        "ApplicationSources": Sequence[ApplicationSourceUnionTypeDef],
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-_RequiredScalingInstructionOutputTypeDef = TypedDict(
-    "_RequiredScalingInstructionOutputTypeDef",
+_RequiredScalingInstructionTypeDef = TypedDict(
+    "_RequiredScalingInstructionTypeDef",
     {
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
         "ScalableDimension": ScalableDimensionType,
         "MinCapacity": int,
         "MaxCapacity": int,
-        "TargetTrackingConfigurations": List[TargetTrackingConfigurationOutputTypeDef],
+        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
     },
 )
-_OptionalScalingInstructionOutputTypeDef = TypedDict(
-    "_OptionalScalingInstructionOutputTypeDef",
+_OptionalScalingInstructionTypeDef = TypedDict(
+    "_OptionalScalingInstructionTypeDef",
     {
         "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationOutputTypeDef,
+        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
         "ScheduledActionBufferTime": int,
         "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
         "PredictiveScalingMaxCapacityBuffer": int,
         "PredictiveScalingMode": PredictiveScalingModeType,
         "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
         "DisableDynamicScaling": bool,
     },
     total=False,
 )
 
-class ScalingInstructionOutputTypeDef(
-    _RequiredScalingInstructionOutputTypeDef, _OptionalScalingInstructionOutputTypeDef
+class ScalingInstructionTypeDef(
+    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
 ):
     pass
 
 _RequiredScalingPolicyTypeDef = TypedDict(
     "_RequiredScalingPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyType": Literal["TargetTrackingScaling"],
     },
 )
 _OptionalScalingPolicyTypeDef = TypedDict(
     "_OptionalScalingPolicyTypeDef",
     {
-        "TargetTrackingConfiguration": TargetTrackingConfigurationOutputTypeDef,
+        "TargetTrackingConfiguration": TargetTrackingConfigurationTypeDef,
     },
     total=False,
 )
 
 class ScalingPolicyTypeDef(_RequiredScalingPolicyTypeDef, _OptionalScalingPolicyTypeDef):
     pass
 
-_RequiredScalingInstructionTypeDef = TypedDict(
-    "_RequiredScalingInstructionTypeDef",
-    {
-        "ServiceNamespace": ServiceNamespaceType,
-        "ResourceId": str,
-        "ScalableDimension": ScalableDimensionType,
-        "MinCapacity": int,
-        "MaxCapacity": int,
-        "TargetTrackingConfigurations": Sequence[TargetTrackingConfigurationTypeDef],
-    },
-)
-_OptionalScalingInstructionTypeDef = TypedDict(
-    "_OptionalScalingInstructionTypeDef",
+CreateScalingPlanRequestRequestTypeDef = TypedDict(
+    "CreateScalingPlanRequestRequestTypeDef",
     {
-        "PredefinedLoadMetricSpecification": PredefinedLoadMetricSpecificationTypeDef,
-        "CustomizedLoadMetricSpecification": CustomizedLoadMetricSpecificationTypeDef,
-        "ScheduledActionBufferTime": int,
-        "PredictiveScalingMaxCapacityBehavior": PredictiveScalingMaxCapacityBehaviorType,
-        "PredictiveScalingMaxCapacityBuffer": int,
-        "PredictiveScalingMode": PredictiveScalingModeType,
-        "ScalingPolicyUpdateBehavior": ScalingPolicyUpdateBehaviorType,
-        "DisableDynamicScaling": bool,
+        "ScalingPlanName": str,
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
     },
-    total=False,
 )
 
-class ScalingInstructionTypeDef(
-    _RequiredScalingInstructionTypeDef, _OptionalScalingInstructionTypeDef
-):
-    pass
-
 _RequiredScalingPlanTypeDef = TypedDict(
     "_RequiredScalingPlanTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
-        "ApplicationSource": ApplicationSourceOutputTypeDef,
-        "ScalingInstructions": List[ScalingInstructionOutputTypeDef],
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": List[ScalingInstructionTypeDef],
         "StatusCode": ScalingPlanStatusCodeType,
     },
 )
 _OptionalScalingPlanTypeDef = TypedDict(
     "_OptionalScalingPlanTypeDef",
     {
         "StatusMessage": str,
@@ -537,14 +417,35 @@
     },
     total=False,
 )
 
 class ScalingPlanTypeDef(_RequiredScalingPlanTypeDef, _OptionalScalingPlanTypeDef):
     pass
 
+_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ScalingPlanName": str,
+        "ScalingPlanVersion": int,
+    },
+)
+_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
+    {
+        "ApplicationSource": ApplicationSourceTypeDef,
+        "ScalingInstructions": Sequence[ScalingInstructionTypeDef],
+    },
+    total=False,
+)
+
+class UpdateScalingPlanRequestRequestTypeDef(
+    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
+):
+    pass
+
 _RequiredScalingPlanResourceTypeDef = TypedDict(
     "_RequiredScalingPlanResourceTypeDef",
     {
         "ScalingPlanName": str,
         "ScalingPlanVersion": int,
         "ServiceNamespace": ServiceNamespaceType,
         "ResourceId": str,
@@ -562,15 +463,14 @@
 )
 
 class ScalingPlanResourceTypeDef(
     _RequiredScalingPlanResourceTypeDef, _OptionalScalingPlanResourceTypeDef
 ):
     pass
 
-ScalingInstructionUnionTypeDef = Union[ScalingInstructionTypeDef, ScalingInstructionOutputTypeDef]
 DescribeScalingPlansResponseTypeDef = TypedDict(
     "DescribeScalingPlansResponseTypeDef",
     {
         "ScalingPlans": List[ScalingPlanTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -580,37 +480,7 @@
     "DescribeScalingPlanResourcesResponseTypeDef",
     {
         "ScalingPlanResources": List[ScalingPlanResourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-CreateScalingPlanRequestRequestTypeDef = TypedDict(
-    "CreateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
-    },
-)
-
-_RequiredUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ScalingPlanName": str,
-        "ScalingPlanVersion": int,
-    },
-)
-_OptionalUpdateScalingPlanRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateScalingPlanRequestRequestTypeDef",
-    {
-        "ApplicationSource": ApplicationSourceTypeDef,
-        "ScalingInstructions": Sequence[ScalingInstructionUnionTypeDef],
-    },
-    total=False,
-)
-
-class UpdateScalingPlanRequestRequestTypeDef(
-    _RequiredUpdateScalingPlanRequestRequestTypeDef, _OptionalUpdateScalingPlanRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/PKG-INFO` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-autoscaling-plans
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AutoScalingPlans 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore autoscaling-plans type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-autoscaling-plans"></a>
 
 # types-aiobotocore-autoscaling-plans
 
 [![PyPI - types-aiobotocore-autoscaling-plans](https://img.shields.io/pypi/v/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-autoscaling-plans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-autoscaling-plans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/)
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
 [types-aiobotocore-autoscaling-plans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,91 +265,40 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_autoscaling_plans.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `AutoScalingPlans` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/literals/).
+
 ```python
-from types_aiobotocore_autoscaling_plans.literals import (
-    DescribeScalingPlanResourcesPaginatorName,
-    DescribeScalingPlansPaginatorName,
-    ForecastDataTypeType,
-    LoadMetricTypeType,
-    MetricStatisticType,
-    PolicyTypeType,
-    PredictiveScalingMaxCapacityBehaviorType,
-    PredictiveScalingModeType,
-    ScalableDimensionType,
-    ScalingMetricTypeType,
-    ScalingPlanStatusCodeType,
-    ScalingPolicyUpdateBehaviorType,
-    ScalingStatusCodeType,
-    ServiceNamespaceType,
-    AutoScalingPlansServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_autoscaling_plans.literals import DescribeScalingPlanResourcesPaginatorName
 
 
 def check_value(value: DescribeScalingPlanResourcesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_autoscaling_plans.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AutoScalingPlans` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_autoscaling_plans/type_defs/).
+
 ```python
-from types_aiobotocore_autoscaling_plans.type_defs import (
-    TagFilterOutputTypeDef,
-    TagFilterTypeDef,
-    ResponseMetadataTypeDef,
-    MetricDimensionTypeDef,
-    DatapointTypeDef,
-    DeleteScalingPlanRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeScalingPlanResourcesRequestRequestTypeDef,
-    TimestampTypeDef,
-    PredefinedLoadMetricSpecificationTypeDef,
-    PredefinedScalingMetricSpecificationTypeDef,
-    ApplicationSourceOutputTypeDef,
-    ApplicationSourceTypeDef,
-    CreateScalingPlanResponseTypeDef,
-    CustomizedLoadMetricSpecificationOutputTypeDef,
-    CustomizedLoadMetricSpecificationTypeDef,
-    CustomizedScalingMetricSpecificationOutputTypeDef,
-    CustomizedScalingMetricSpecificationTypeDef,
-    GetScalingPlanResourceForecastDataResponseTypeDef,
-    DescribeScalingPlanResourcesRequestDescribeScalingPlanResourcesPaginateTypeDef,
-    GetScalingPlanResourceForecastDataRequestRequestTypeDef,
-    ApplicationSourceUnionTypeDef,
-    TargetTrackingConfigurationOutputTypeDef,
-    TargetTrackingConfigurationTypeDef,
-    DescribeScalingPlansRequestDescribeScalingPlansPaginateTypeDef,
-    DescribeScalingPlansRequestRequestTypeDef,
-    ScalingInstructionOutputTypeDef,
-    ScalingPolicyTypeDef,
-    ScalingInstructionTypeDef,
-    ScalingPlanTypeDef,
-    ScalingPlanResourceTypeDef,
-    ScalingInstructionUnionTypeDef,
-    DescribeScalingPlansResponseTypeDef,
-    DescribeScalingPlanResourcesResponseTypeDef,
-    CreateScalingPlanRequestRequestTypeDef,
-    UpdateScalingPlanRequestRequestTypeDef,
-)
+from types_aiobotocore_autoscaling_plans.type_defs import TagFilterTypeDef
 
 
-def get_value() -> TagFilterOutputTypeDef:
+def get_value() -> TagFilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-autoscaling-plans-2.5.2.post1/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt` & `types-aiobotocore-autoscaling-plans-2.5.2.post2/types_aiobotocore_autoscaling_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

