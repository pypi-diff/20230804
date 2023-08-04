# Comparing `tmp/types-aiobotocore-datapipeline-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-datapipeline-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datapipeline-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-datapipeline-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-datapipeline-2.5.2.post1.tar` & `types-aiobotocore-datapipeline-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.593608 types-aiobotocore-datapipeline-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-08-02 14:52:09.593608 types-aiobotocore-datapipeline-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.593608 types-aiobotocore-datapipeline-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.589608 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18120 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18089 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-08-02 14:36:08.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-08-02 14:36:08.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-08-02 14:36:08.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-08-02 14:36:08.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:07.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.593608 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-08-02 14:52:09.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:09.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:09.000000 types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.483841 types-aiobotocore-datapipeline-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-08-04 12:00:44.483841 types-aiobotocore-datapipeline-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.483841 types-aiobotocore-datapipeline-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.479841 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18059 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8231 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8229 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17951 2023-08-04 11:43:28.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17919 2023-08-04 11:43:28.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:27.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.483841 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13467 2023-08-04 12:00:44.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-04 12:00:44.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 12:00:44.000000 types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/LICENSE` & `types-aiobotocore-datapipeline-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/PKG-INFO` & `types-aiobotocore-datapipeline-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datapipeline
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/
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
 [types-aiobotocore-datapipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,100 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_datapipeline.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DataPipeline` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/literals/).
+
 ```python
-from types_aiobotocore_datapipeline.literals import (
-    DescribeObjectsPaginatorName,
-    ListPipelinesPaginatorName,
-    OperatorTypeType,
-    QueryObjectsPaginatorName,
-    TaskStatusType,
-    DataPipelineServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_datapipeline.literals import DescribeObjectsPaginatorName
 
 
 def check_value(value: DescribeObjectsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_datapipeline.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DataPipeline` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/type_defs/).
+
 ```python
-from types_aiobotocore_datapipeline.type_defs import (
-    ParameterValueTypeDef,
-    TimestampTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeactivatePipelineInputRequestTypeDef,
-    DeletePipelineInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeObjectsInputRequestTypeDef,
-    DescribePipelinesInputRequestTypeDef,
-    EvaluateExpressionInputRequestTypeDef,
-    FieldTypeDef,
-    GetPipelineDefinitionInputRequestTypeDef,
-    InstanceIdentityTypeDef,
-    ListPipelinesInputRequestTypeDef,
-    PipelineIdNameTypeDef,
-    OperatorTypeDef,
-    ParameterAttributeTypeDef,
-    ValidationErrorTypeDef,
-    ValidationWarningTypeDef,
-    RemoveTagsInputRequestTypeDef,
-    ReportTaskRunnerHeartbeatInputRequestTypeDef,
-    SetStatusInputRequestTypeDef,
-    SetTaskStatusInputRequestTypeDef,
-    ActivatePipelineInputRequestTypeDef,
-    AddTagsInputRequestTypeDef,
-    CreatePipelineInputRequestTypeDef,
-    CreatePipelineOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    QueryObjectsOutputTypeDef,
-    ReportTaskProgressOutputTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
-    PipelineDescriptionTypeDef,
-    PipelineObjectOutputTypeDef,
-    PipelineObjectTypeDef,
-    ReportTaskProgressInputRequestTypeDef,
-    PollForTaskInputRequestTypeDef,
-    ListPipelinesOutputTypeDef,
-    SelectorTypeDef,
-    ParameterObjectOutputTypeDef,
-    ParameterObjectTypeDef,
-    PutPipelineDefinitionOutputTypeDef,
-    ValidatePipelineDefinitionOutputTypeDef,
-    DescribePipelinesOutputTypeDef,
-    DescribeObjectsOutputTypeDef,
-    TaskObjectTypeDef,
-    PipelineObjectUnionTypeDef,
-    QueryTypeDef,
-    GetPipelineDefinitionOutputTypeDef,
-    ParameterObjectUnionTypeDef,
-    PollForTaskOutputTypeDef,
-    QueryObjectsInputQueryObjectsPaginateTypeDef,
-    QueryObjectsInputRequestTypeDef,
-    PutPipelineDefinitionInputRequestTypeDef,
-    ValidatePipelineDefinitionInputRequestTypeDef,
-)
+from types_aiobotocore_datapipeline.type_defs import ParameterValueTypeDef
 
 
 def get_value() -> ParameterValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/README.md` & `types-aiobotocore-datapipeline-2.5.2.post2/README.md`

 * *Files 17% similar despite different names*

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
 [types-aiobotocore-datapipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,100 +263,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_datapipeline.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DataPipeline` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/literals/).
+
 ```python
-from types_aiobotocore_datapipeline.literals import (
-    DescribeObjectsPaginatorName,
-    ListPipelinesPaginatorName,
-    OperatorTypeType,
-    QueryObjectsPaginatorName,
-    TaskStatusType,
-    DataPipelineServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_datapipeline.literals import DescribeObjectsPaginatorName
 
 
 def check_value(value: DescribeObjectsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_datapipeline.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DataPipeline` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/type_defs/).
+
 ```python
-from types_aiobotocore_datapipeline.type_defs import (
-    ParameterValueTypeDef,
-    TimestampTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeactivatePipelineInputRequestTypeDef,
-    DeletePipelineInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeObjectsInputRequestTypeDef,
-    DescribePipelinesInputRequestTypeDef,
-    EvaluateExpressionInputRequestTypeDef,
-    FieldTypeDef,
-    GetPipelineDefinitionInputRequestTypeDef,
-    InstanceIdentityTypeDef,
-    ListPipelinesInputRequestTypeDef,
-    PipelineIdNameTypeDef,
-    OperatorTypeDef,
-    ParameterAttributeTypeDef,
-    ValidationErrorTypeDef,
-    ValidationWarningTypeDef,
-    RemoveTagsInputRequestTypeDef,
-    ReportTaskRunnerHeartbeatInputRequestTypeDef,
-    SetStatusInputRequestTypeDef,
-    SetTaskStatusInputRequestTypeDef,
-    ActivatePipelineInputRequestTypeDef,
-    AddTagsInputRequestTypeDef,
-    CreatePipelineInputRequestTypeDef,
-    CreatePipelineOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    QueryObjectsOutputTypeDef,
-    ReportTaskProgressOutputTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
-    PipelineDescriptionTypeDef,
-    PipelineObjectOutputTypeDef,
-    PipelineObjectTypeDef,
-    ReportTaskProgressInputRequestTypeDef,
-    PollForTaskInputRequestTypeDef,
-    ListPipelinesOutputTypeDef,
-    SelectorTypeDef,
-    ParameterObjectOutputTypeDef,
-    ParameterObjectTypeDef,
-    PutPipelineDefinitionOutputTypeDef,
-    ValidatePipelineDefinitionOutputTypeDef,
-    DescribePipelinesOutputTypeDef,
-    DescribeObjectsOutputTypeDef,
-    TaskObjectTypeDef,
-    PipelineObjectUnionTypeDef,
-    QueryTypeDef,
-    GetPipelineDefinitionOutputTypeDef,
-    ParameterObjectUnionTypeDef,
-    PollForTaskOutputTypeDef,
-    QueryObjectsInputQueryObjectsPaginateTypeDef,
-    QueryObjectsInputRequestTypeDef,
-    PutPipelineDefinitionInputRequestTypeDef,
-    ValidatePipelineDefinitionInputRequestTypeDef,
-)
+from types_aiobotocore_datapipeline.type_defs import ParameterValueTypeDef
 
 
 def get_value() -> ParameterValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/setup.py` & `types-aiobotocore-datapipeline-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datapipeline",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/__init__.py` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/__init__.pyi` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/__main__.py` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataPipeline 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DataPipeline 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/client.py` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     DescribePipelinesOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesOutputTypeDef,
-    ParameterObjectUnionTypeDef,
+    ParameterObjectTypeDef,
     ParameterValueTypeDef,
-    PipelineObjectUnionTypeDef,
+    PipelineObjectTypeDef,
     PollForTaskOutputTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     TagTypeDef,
@@ -239,16 +239,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#poll_for_task)
         """
 
     async def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
-        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
+        pipelineObjects: Sequence[PipelineObjectTypeDef],
+        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#put_pipeline_definition)
@@ -329,16 +329,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#set_task_status)
         """
 
     async def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
-        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
+        pipelineObjects: Sequence[PipelineObjectTypeDef],
+        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed and
         can be run without error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/client.pyi` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     DescribePipelinesOutputTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluateExpressionOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     InstanceIdentityTypeDef,
     ListPipelinesOutputTypeDef,
-    ParameterObjectUnionTypeDef,
+    ParameterObjectTypeDef,
     ParameterValueTypeDef,
-    PipelineObjectUnionTypeDef,
+    PipelineObjectTypeDef,
     PollForTaskOutputTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
     ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatOutputTypeDef,
     TagTypeDef,
@@ -220,16 +220,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#poll_for_task)
         """
     async def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
-        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
+        pipelineObjects: Sequence[PipelineObjectTypeDef],
+        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#put_pipeline_definition)
@@ -303,16 +303,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#set_task_status)
         """
     async def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
-        pipelineObjects: Sequence[PipelineObjectUnionTypeDef],
-        parameterObjects: Sequence[ParameterObjectUnionTypeDef] = ...,
+        pipelineObjects: Sequence[PipelineObjectTypeDef],
+        parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
         parameterValues: Sequence[ParameterValueTypeDef] = ...
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed and
         can be run without error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/literals.py` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/literals.pyi` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/paginator.py` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/paginator.pyi` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/type_defs.py` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from .literals import OperatorTypeType, TaskStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ParameterValueTypeDef",
     "TimestampTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
@@ -55,36 +54,32 @@
     "EvaluateExpressionOutputTypeDef",
     "QueryObjectsOutputTypeDef",
     "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatOutputTypeDef",
     "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "PipelineDescriptionTypeDef",
-    "PipelineObjectOutputTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
-    "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
     "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
-    "PipelineObjectUnionTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
-    "ParameterObjectUnionTypeDef",
+    "PutPipelineDefinitionInputRequestTypeDef",
+    "ValidatePipelineDefinitionInputRequestTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
-    "PutPipelineDefinitionInputRequestTypeDef",
-    "ValidatePipelineDefinitionInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "id": str,
         "stringValue": str,
@@ -121,21 +116,19 @@
     "_OptionalDeactivatePipelineInputRequestTypeDef",
     {
         "cancelActive": bool,
     },
     total=False,
 )
 
-
 class DeactivatePipelineInputRequestTypeDef(
     _RequiredDeactivatePipelineInputRequestTypeDef, _OptionalDeactivatePipelineInputRequestTypeDef
 ):
     pass
 
-
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
@@ -161,21 +154,19 @@
     {
         "evaluateExpressions": bool,
         "marker": str,
     },
     total=False,
 )
 
-
 class DescribeObjectsInputRequestTypeDef(
     _RequiredDescribeObjectsInputRequestTypeDef, _OptionalDescribeObjectsInputRequestTypeDef
 ):
     pass
 
-
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
@@ -199,41 +190,37 @@
     {
         "stringValue": str,
         "refValue": str,
     },
     total=False,
 )
 
-
 class FieldTypeDef(_RequiredFieldTypeDef, _OptionalFieldTypeDef):
     pass
 
-
 _RequiredGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredGetPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalGetPipelineDefinitionInputRequestTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
-
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
@@ -310,22 +297,20 @@
     {
         "workerGroup": str,
         "hostname": str,
     },
     total=False,
 )
 
-
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
-
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -344,21 +329,19 @@
         "errorId": str,
         "errorMessage": str,
         "errorStackTrace": str,
     },
     total=False,
 )
 
-
 class SetTaskStatusInputRequestTypeDef(
     _RequiredSetTaskStatusInputRequestTypeDef, _OptionalSetTaskStatusInputRequestTypeDef
 ):
     pass
 
-
 _RequiredActivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredActivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalActivatePipelineInputRequestTypeDef = TypedDict(
@@ -366,21 +349,19 @@
     {
         "parameterValues": Sequence[ParameterValueTypeDef],
         "startTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class ActivatePipelineInputRequestTypeDef(
     _RequiredActivatePipelineInputRequestTypeDef, _OptionalActivatePipelineInputRequestTypeDef
 ):
     pass
 
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -397,21 +378,19 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
-
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipelineId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -469,22 +448,20 @@
     {
         "evaluateExpressions": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
     _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
     _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
 ):
     pass
 
-
 ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -502,36 +479,25 @@
     {
         "description": str,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class PipelineDescriptionTypeDef(
     _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
 ):
     pass
 
-
-PipelineObjectOutputTypeDef = TypedDict(
-    "PipelineObjectOutputTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "fields": List[FieldTypeDef],
-    },
-)
-
 PipelineObjectTypeDef = TypedDict(
     "PipelineObjectTypeDef",
     {
         "id": str,
         "name": str,
-        "fields": Sequence[FieldTypeDef],
+        "fields": List[FieldTypeDef],
     },
 )
 
 _RequiredReportTaskProgressInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskProgressInputRequestTypeDef",
     {
         "taskId": str,
@@ -541,21 +507,19 @@
     "_OptionalReportTaskProgressInputRequestTypeDef",
     {
         "fields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
-
 class ReportTaskProgressInputRequestTypeDef(
     _RequiredReportTaskProgressInputRequestTypeDef, _OptionalReportTaskProgressInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPollForTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForTaskInputRequestTypeDef",
     {
         "workerGroup": str,
     },
 )
 _OptionalPollForTaskInputRequestTypeDef = TypedDict(
@@ -563,21 +527,19 @@
     {
         "hostname": str,
         "instanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
-
 class PollForTaskInputRequestTypeDef(
     _RequiredPollForTaskInputRequestTypeDef, _OptionalPollForTaskInputRequestTypeDef
 ):
     pass
 
-
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -589,27 +551,19 @@
     {
         "fieldName": str,
         "operator": OperatorTypeDef,
     },
     total=False,
 )
 
-ParameterObjectOutputTypeDef = TypedDict(
-    "ParameterObjectOutputTypeDef",
-    {
-        "id": str,
-        "attributes": List[ParameterAttributeTypeDef],
-    },
-)
-
 ParameterObjectTypeDef = TypedDict(
     "ParameterObjectTypeDef",
     {
         "id": str,
-        "attributes": Sequence[ParameterAttributeTypeDef],
+        "attributes": List[ParameterAttributeTypeDef],
     },
 )
 
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
@@ -636,52 +590,94 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectOutputTypeDef],
+        "pipelineObjects": List[PipelineObjectTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
         "pipelineId": str,
         "attemptId": str,
-        "objects": Dict[str, PipelineObjectOutputTypeDef],
+        "objects": Dict[str, PipelineObjectTypeDef],
     },
     total=False,
 )
 
-PipelineObjectUnionTypeDef = Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "selectors": Sequence[SelectorTypeDef],
     },
     total=False,
 )
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectOutputTypeDef],
-        "parameterObjects": List[ParameterObjectOutputTypeDef],
+        "pipelineObjects": List[PipelineObjectTypeDef],
+        "parameterObjects": List[ParameterObjectTypeDef],
         "parameterValues": List[ParameterValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ParameterObjectUnionTypeDef = Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
+_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+    },
+)
+_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+class PutPipelineDefinitionInputRequestTypeDef(
+    _RequiredPutPipelineDefinitionInputRequestTypeDef,
+    _OptionalPutPipelineDefinitionInputRequestTypeDef,
+):
+    pass
+
+_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+    },
+)
+_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+class ValidatePipelineDefinitionInputRequestTypeDef(
+    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
+    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
+):
+    pass
+
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -698,22 +694,20 @@
     {
         "query": QueryTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredQueryObjectsInputRequestTypeDef = TypedDict(
     "_RequiredQueryObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
@@ -723,60 +717,11 @@
         "query": QueryTypeDef,
         "marker": str,
         "limit": int,
     },
     total=False,
 )
 
-
 class QueryObjectsInputRequestTypeDef(
     _RequiredQueryObjectsInputRequestTypeDef, _OptionalQueryObjectsInputRequestTypeDef
 ):
     pass
-
-
-_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
-    },
-)
-_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-
-class PutPipelineDefinitionInputRequestTypeDef(
-    _RequiredPutPipelineDefinitionInputRequestTypeDef,
-    _OptionalPutPipelineDefinitionInputRequestTypeDef,
-):
-    pass
-
-
-_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
-    },
-)
-_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-
-class ValidatePipelineDefinitionInputRequestTypeDef(
-    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
-    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline/type_defs.pyi` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from .literals import OperatorTypeType, TaskStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ParameterValueTypeDef",
     "TimestampTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
@@ -54,36 +55,32 @@
     "EvaluateExpressionOutputTypeDef",
     "QueryObjectsOutputTypeDef",
     "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatOutputTypeDef",
     "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     "PipelineDescriptionTypeDef",
-    "PipelineObjectOutputTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
-    "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
     "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
-    "PipelineObjectUnionTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
-    "ParameterObjectUnionTypeDef",
+    "PutPipelineDefinitionInputRequestTypeDef",
+    "ValidatePipelineDefinitionInputRequestTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
-    "PutPipelineDefinitionInputRequestTypeDef",
-    "ValidatePipelineDefinitionInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
     {
         "id": str,
         "stringValue": str,
@@ -120,19 +117,21 @@
     "_OptionalDeactivatePipelineInputRequestTypeDef",
     {
         "cancelActive": bool,
     },
     total=False,
 )
 
+
 class DeactivatePipelineInputRequestTypeDef(
     _RequiredDeactivatePipelineInputRequestTypeDef, _OptionalDeactivatePipelineInputRequestTypeDef
 ):
     pass
 
+
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
@@ -158,19 +157,21 @@
     {
         "evaluateExpressions": bool,
         "marker": str,
     },
     total=False,
 )
 
+
 class DescribeObjectsInputRequestTypeDef(
     _RequiredDescribeObjectsInputRequestTypeDef, _OptionalDescribeObjectsInputRequestTypeDef
 ):
     pass
 
+
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
@@ -194,37 +195,41 @@
     {
         "stringValue": str,
         "refValue": str,
     },
     total=False,
 )
 
+
 class FieldTypeDef(_RequiredFieldTypeDef, _OptionalFieldTypeDef):
     pass
 
+
 _RequiredGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredGetPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalGetPipelineDefinitionInputRequestTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
+
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
+
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
@@ -301,20 +306,22 @@
     {
         "workerGroup": str,
         "hostname": str,
     },
     total=False,
 )
 
+
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
+
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -333,19 +340,21 @@
         "errorId": str,
         "errorMessage": str,
         "errorStackTrace": str,
     },
     total=False,
 )
 
+
 class SetTaskStatusInputRequestTypeDef(
     _RequiredSetTaskStatusInputRequestTypeDef, _OptionalSetTaskStatusInputRequestTypeDef
 ):
     pass
 
+
 _RequiredActivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredActivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalActivatePipelineInputRequestTypeDef = TypedDict(
@@ -353,19 +362,21 @@
     {
         "parameterValues": Sequence[ParameterValueTypeDef],
         "startTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class ActivatePipelineInputRequestTypeDef(
     _RequiredActivatePipelineInputRequestTypeDef, _OptionalActivatePipelineInputRequestTypeDef
 ):
     pass
 
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -382,19 +393,21 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+
 CreatePipelineOutputTypeDef = TypedDict(
     "CreatePipelineOutputTypeDef",
     {
         "pipelineId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -452,20 +465,22 @@
     {
         "evaluateExpressions": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
     _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
     _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
 ):
     pass
 
+
 ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
     "ListPipelinesInputListPipelinesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -483,34 +498,27 @@
     {
         "description": str,
         "tags": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class PipelineDescriptionTypeDef(
     _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
 ):
     pass
 
-PipelineObjectOutputTypeDef = TypedDict(
-    "PipelineObjectOutputTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "fields": List[FieldTypeDef],
-    },
-)
 
 PipelineObjectTypeDef = TypedDict(
     "PipelineObjectTypeDef",
     {
         "id": str,
         "name": str,
-        "fields": Sequence[FieldTypeDef],
+        "fields": List[FieldTypeDef],
     },
 )
 
 _RequiredReportTaskProgressInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskProgressInputRequestTypeDef",
     {
         "taskId": str,
@@ -520,19 +528,21 @@
     "_OptionalReportTaskProgressInputRequestTypeDef",
     {
         "fields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
+
 class ReportTaskProgressInputRequestTypeDef(
     _RequiredReportTaskProgressInputRequestTypeDef, _OptionalReportTaskProgressInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPollForTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForTaskInputRequestTypeDef",
     {
         "workerGroup": str,
     },
 )
 _OptionalPollForTaskInputRequestTypeDef = TypedDict(
@@ -540,19 +550,21 @@
     {
         "hostname": str,
         "instanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
+
 class PollForTaskInputRequestTypeDef(
     _RequiredPollForTaskInputRequestTypeDef, _OptionalPollForTaskInputRequestTypeDef
 ):
     pass
 
+
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -564,27 +576,19 @@
     {
         "fieldName": str,
         "operator": OperatorTypeDef,
     },
     total=False,
 )
 
-ParameterObjectOutputTypeDef = TypedDict(
-    "ParameterObjectOutputTypeDef",
-    {
-        "id": str,
-        "attributes": List[ParameterAttributeTypeDef],
-    },
-)
-
 ParameterObjectTypeDef = TypedDict(
     "ParameterObjectTypeDef",
     {
         "id": str,
-        "attributes": Sequence[ParameterAttributeTypeDef],
+        "attributes": List[ParameterAttributeTypeDef],
     },
 )
 
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
@@ -611,52 +615,98 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectOutputTypeDef],
+        "pipelineObjects": List[PipelineObjectTypeDef],
         "marker": str,
         "hasMoreResults": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
         "pipelineId": str,
         "attemptId": str,
-        "objects": Dict[str, PipelineObjectOutputTypeDef],
+        "objects": Dict[str, PipelineObjectTypeDef],
     },
     total=False,
 )
 
-PipelineObjectUnionTypeDef = Union[PipelineObjectTypeDef, PipelineObjectOutputTypeDef]
 QueryTypeDef = TypedDict(
     "QueryTypeDef",
     {
         "selectors": Sequence[SelectorTypeDef],
     },
     total=False,
 )
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
-        "pipelineObjects": List[PipelineObjectOutputTypeDef],
-        "parameterObjects": List[ParameterObjectOutputTypeDef],
+        "pipelineObjects": List[PipelineObjectTypeDef],
+        "parameterObjects": List[ParameterObjectTypeDef],
         "parameterValues": List[ParameterValueTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ParameterObjectUnionTypeDef = Union[ParameterObjectTypeDef, ParameterObjectOutputTypeDef]
+_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+    },
+)
+_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+
+class PutPipelineDefinitionInputRequestTypeDef(
+    _RequiredPutPipelineDefinitionInputRequestTypeDef,
+    _OptionalPutPipelineDefinitionInputRequestTypeDef,
+):
+    pass
+
+
+_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "pipelineId": str,
+        "pipelineObjects": Sequence[PipelineObjectTypeDef],
+    },
+)
+_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
+    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
+    {
+        "parameterObjects": Sequence[ParameterObjectTypeDef],
+        "parameterValues": Sequence[ParameterValueTypeDef],
+    },
+    total=False,
+)
+
+
+class ValidatePipelineDefinitionInputRequestTypeDef(
+    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
+    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
+):
+    pass
+
+
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -673,20 +723,22 @@
     {
         "query": QueryTypeDef,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredQueryObjectsInputRequestTypeDef = TypedDict(
     "_RequiredQueryObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
@@ -696,55 +748,12 @@
         "query": QueryTypeDef,
         "marker": str,
         "limit": int,
     },
     total=False,
 )
 
+
 class QueryObjectsInputRequestTypeDef(
     _RequiredQueryObjectsInputRequestTypeDef, _OptionalQueryObjectsInputRequestTypeDef
 ):
     pass
-
-_RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
-    },
-)
-_OptionalPutPipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalPutPipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-class PutPipelineDefinitionInputRequestTypeDef(
-    _RequiredPutPipelineDefinitionInputRequestTypeDef,
-    _OptionalPutPipelineDefinitionInputRequestTypeDef,
-):
-    pass
-
-_RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "pipelineId": str,
-        "pipelineObjects": Sequence[PipelineObjectUnionTypeDef],
-    },
-)
-_OptionalValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
-    "_OptionalValidatePipelineDefinitionInputRequestTypeDef",
-    {
-        "parameterObjects": Sequence[ParameterObjectUnionTypeDef],
-        "parameterValues": Sequence[ParameterValueTypeDef],
-    },
-    total=False,
-)
-
-class ValidatePipelineDefinitionInputRequestTypeDef(
-    _RequiredValidatePipelineDefinitionInputRequestTypeDef,
-    _OptionalValidatePipelineDefinitionInputRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/PKG-INFO` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datapipeline
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DataPipeline 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/
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
 [types-aiobotocore-datapipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,100 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_datapipeline.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DataPipeline` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/literals/).
+
 ```python
-from types_aiobotocore_datapipeline.literals import (
-    DescribeObjectsPaginatorName,
-    ListPipelinesPaginatorName,
-    OperatorTypeType,
-    QueryObjectsPaginatorName,
-    TaskStatusType,
-    DataPipelineServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_datapipeline.literals import DescribeObjectsPaginatorName
 
 
 def check_value(value: DescribeObjectsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_datapipeline.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DataPipeline` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/type_defs/).
+
 ```python
-from types_aiobotocore_datapipeline.type_defs import (
-    ParameterValueTypeDef,
-    TimestampTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeactivatePipelineInputRequestTypeDef,
-    DeletePipelineInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeObjectsInputRequestTypeDef,
-    DescribePipelinesInputRequestTypeDef,
-    EvaluateExpressionInputRequestTypeDef,
-    FieldTypeDef,
-    GetPipelineDefinitionInputRequestTypeDef,
-    InstanceIdentityTypeDef,
-    ListPipelinesInputRequestTypeDef,
-    PipelineIdNameTypeDef,
-    OperatorTypeDef,
-    ParameterAttributeTypeDef,
-    ValidationErrorTypeDef,
-    ValidationWarningTypeDef,
-    RemoveTagsInputRequestTypeDef,
-    ReportTaskRunnerHeartbeatInputRequestTypeDef,
-    SetStatusInputRequestTypeDef,
-    SetTaskStatusInputRequestTypeDef,
-    ActivatePipelineInputRequestTypeDef,
-    AddTagsInputRequestTypeDef,
-    CreatePipelineInputRequestTypeDef,
-    CreatePipelineOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    QueryObjectsOutputTypeDef,
-    ReportTaskProgressOutputTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
-    PipelineDescriptionTypeDef,
-    PipelineObjectOutputTypeDef,
-    PipelineObjectTypeDef,
-    ReportTaskProgressInputRequestTypeDef,
-    PollForTaskInputRequestTypeDef,
-    ListPipelinesOutputTypeDef,
-    SelectorTypeDef,
-    ParameterObjectOutputTypeDef,
-    ParameterObjectTypeDef,
-    PutPipelineDefinitionOutputTypeDef,
-    ValidatePipelineDefinitionOutputTypeDef,
-    DescribePipelinesOutputTypeDef,
-    DescribeObjectsOutputTypeDef,
-    TaskObjectTypeDef,
-    PipelineObjectUnionTypeDef,
-    QueryTypeDef,
-    GetPipelineDefinitionOutputTypeDef,
-    ParameterObjectUnionTypeDef,
-    PollForTaskOutputTypeDef,
-    QueryObjectsInputQueryObjectsPaginateTypeDef,
-    QueryObjectsInputRequestTypeDef,
-    PutPipelineDefinitionInputRequestTypeDef,
-    ValidatePipelineDefinitionInputRequestTypeDef,
-)
+from types_aiobotocore_datapipeline.type_defs import ParameterValueTypeDef
 
 
 def get_value() -> ParameterValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-datapipeline-2.5.2.post1/types_aiobotocore_datapipeline.egg-info/SOURCES.txt` & `types-aiobotocore-datapipeline-2.5.2.post2/types_aiobotocore_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

