# Comparing `tmp/types-aiobotocore-dax-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-dax-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dax-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-dax-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:44 2023, max compression
```

## Comparing `types-aiobotocore-dax-2.5.2.post1.tar` & `types-aiobotocore-dax-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.677607 types-aiobotocore-dax-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-08-02 14:52:09.673607 types-aiobotocore-dax-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14948 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.677607 types-aiobotocore-dax-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.673607 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21992 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-08-02 14:36:13.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22374 2023-08-02 14:36:13.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:12.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.673607 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16450 2023-08-02 14:52:09.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:09.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:09.000000 types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.647848 types-aiobotocore-dax-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-08-04 12:00:44.643848 types-aiobotocore-dax-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12086 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:44.647848 types-aiobotocore-dax-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.635847 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21992 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21955 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22397 2023-08-04 11:43:33.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22374 2023-08-04 11:43:33.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:43:32.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:44.643848 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13588 2023-08-04 12:00:44.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-04 12:00:44.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:44.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:44.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:44.000000 types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dax-2.5.2.post1/LICENSE` & `types-aiobotocore-dax-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/PKG-INFO` & `types-aiobotocore-dax-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dax
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
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
 [types-aiobotocore-dax docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,119 +311,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dax.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `DAX` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/literals/).
+
 ```python
-from types_aiobotocore_dax.literals import (
-    ChangeTypeType,
-    ClusterEndpointEncryptionTypeType,
-    DescribeClustersPaginatorName,
-    DescribeDefaultParametersPaginatorName,
-    DescribeEventsPaginatorName,
-    DescribeParameterGroupsPaginatorName,
-    DescribeParametersPaginatorName,
-    DescribeSubnetGroupsPaginatorName,
-    IsModifiableType,
-    ListTagsPaginatorName,
-    ParameterTypeType,
-    SSEStatusType,
-    SourceTypeType,
-    DAXServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_dax.literals import ChangeTypeType
 
 
 def check_value(value: ChangeTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dax.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DAX` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/type_defs/).
+
 ```python
-from types_aiobotocore_dax.type_defs import (
-    EndpointTypeDef,
-    NotificationConfigurationTypeDef,
-    ParameterGroupStatusTypeDef,
-    SSEDescriptionTypeDef,
-    SecurityGroupMembershipTypeDef,
-    SSESpecificationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateParameterGroupRequestRequestTypeDef,
-    ParameterGroupTypeDef,
-    CreateSubnetGroupRequestRequestTypeDef,
-    DecreaseReplicationFactorRequestRequestTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteParameterGroupRequestRequestTypeDef,
-    DeleteSubnetGroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeClustersRequestRequestTypeDef,
-    DescribeDefaultParametersRequestRequestTypeDef,
-    TimestampTypeDef,
-    EventTypeDef,
-    DescribeParameterGroupsRequestRequestTypeDef,
-    DescribeParametersRequestRequestTypeDef,
-    DescribeSubnetGroupsRequestRequestTypeDef,
-    IncreaseReplicationFactorRequestRequestTypeDef,
-    ListTagsRequestRequestTypeDef,
-    NodeTypeSpecificValueTypeDef,
-    ParameterNameValueTypeDef,
-    RebootNodeRequestRequestTypeDef,
-    SubnetTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateClusterRequestRequestTypeDef,
-    UpdateSubnetGroupRequestRequestTypeDef,
-    NodeTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
-    ListTagsResponseTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
-    CreateParameterGroupResponseTypeDef,
-    DescribeParameterGroupsResponseTypeDef,
-    UpdateParameterGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeEventsRequestRequestTypeDef,
-    DescribeEventsResponseTypeDef,
-    ParameterTypeDef,
-    UpdateParameterGroupRequestRequestTypeDef,
-    SubnetGroupTypeDef,
-    ClusterTypeDef,
-    DescribeDefaultParametersResponseTypeDef,
-    DescribeParametersResponseTypeDef,
-    CreateSubnetGroupResponseTypeDef,
-    DescribeSubnetGroupsResponseTypeDef,
-    UpdateSubnetGroupResponseTypeDef,
-    CreateClusterResponseTypeDef,
-    DecreaseReplicationFactorResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DescribeClustersResponseTypeDef,
-    IncreaseReplicationFactorResponseTypeDef,
-    RebootNodeResponseTypeDef,
-    UpdateClusterResponseTypeDef,
-)
+from types_aiobotocore_dax.type_defs import EndpointTypeDef
 
 
 def get_value() -> EndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dax-2.5.2.post1/README.md` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-dax
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore dax type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dax"></a>
 
 # types-aiobotocore-dax
 
 [![PyPI - types-aiobotocore-dax](https://img.shields.io/pypi/v/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
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
 [types-aiobotocore-dax docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,119 +311,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dax.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `DAX` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/literals/).
+
 ```python
-from types_aiobotocore_dax.literals import (
-    ChangeTypeType,
-    ClusterEndpointEncryptionTypeType,
-    DescribeClustersPaginatorName,
-    DescribeDefaultParametersPaginatorName,
-    DescribeEventsPaginatorName,
-    DescribeParameterGroupsPaginatorName,
-    DescribeParametersPaginatorName,
-    DescribeSubnetGroupsPaginatorName,
-    IsModifiableType,
-    ListTagsPaginatorName,
-    ParameterTypeType,
-    SSEStatusType,
-    SourceTypeType,
-    DAXServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_dax.literals import ChangeTypeType
 
 
 def check_value(value: ChangeTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dax.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DAX` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/type_defs/).
+
 ```python
-from types_aiobotocore_dax.type_defs import (
-    EndpointTypeDef,
-    NotificationConfigurationTypeDef,
-    ParameterGroupStatusTypeDef,
-    SSEDescriptionTypeDef,
-    SecurityGroupMembershipTypeDef,
-    SSESpecificationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateParameterGroupRequestRequestTypeDef,
-    ParameterGroupTypeDef,
-    CreateSubnetGroupRequestRequestTypeDef,
-    DecreaseReplicationFactorRequestRequestTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteParameterGroupRequestRequestTypeDef,
-    DeleteSubnetGroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeClustersRequestRequestTypeDef,
-    DescribeDefaultParametersRequestRequestTypeDef,
-    TimestampTypeDef,
-    EventTypeDef,
-    DescribeParameterGroupsRequestRequestTypeDef,
-    DescribeParametersRequestRequestTypeDef,
-    DescribeSubnetGroupsRequestRequestTypeDef,
-    IncreaseReplicationFactorRequestRequestTypeDef,
-    ListTagsRequestRequestTypeDef,
-    NodeTypeSpecificValueTypeDef,
-    ParameterNameValueTypeDef,
-    RebootNodeRequestRequestTypeDef,
-    SubnetTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateClusterRequestRequestTypeDef,
-    UpdateSubnetGroupRequestRequestTypeDef,
-    NodeTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
-    ListTagsResponseTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
-    CreateParameterGroupResponseTypeDef,
-    DescribeParameterGroupsResponseTypeDef,
-    UpdateParameterGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeEventsRequestRequestTypeDef,
-    DescribeEventsResponseTypeDef,
-    ParameterTypeDef,
-    UpdateParameterGroupRequestRequestTypeDef,
-    SubnetGroupTypeDef,
-    ClusterTypeDef,
-    DescribeDefaultParametersResponseTypeDef,
-    DescribeParametersResponseTypeDef,
-    CreateSubnetGroupResponseTypeDef,
-    DescribeSubnetGroupsResponseTypeDef,
-    UpdateSubnetGroupResponseTypeDef,
-    CreateClusterResponseTypeDef,
-    DecreaseReplicationFactorResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DescribeClustersResponseTypeDef,
-    IncreaseReplicationFactorResponseTypeDef,
-    RebootNodeResponseTypeDef,
-    UpdateClusterResponseTypeDef,
-)
+from types_aiobotocore_dax.type_defs import EndpointTypeDef
 
 
 def get_value() -> EndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dax-2.5.2.post1/setup.py` & `types-aiobotocore-dax-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dax",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/__init__.py` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/__init__.pyi` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/__main__.py` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DAX 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DAX 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/client.py` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/client.pyi` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/literals.py` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/literals.pyi` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/paginator.py` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/paginator.pyi` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/type_defs.py` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax/type_defs.pyi` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/PKG-INFO` & `types-aiobotocore-dax-2.5.2.post2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-dax
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DAX 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dax type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dax"></a>
 
 # types-aiobotocore-dax
 
 [![PyPI - types-aiobotocore-dax](https://img.shields.io/pypi/v/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
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
 [types-aiobotocore-dax docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,119 +279,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dax.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `DAX` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/literals/).
+
 ```python
-from types_aiobotocore_dax.literals import (
-    ChangeTypeType,
-    ClusterEndpointEncryptionTypeType,
-    DescribeClustersPaginatorName,
-    DescribeDefaultParametersPaginatorName,
-    DescribeEventsPaginatorName,
-    DescribeParameterGroupsPaginatorName,
-    DescribeParametersPaginatorName,
-    DescribeSubnetGroupsPaginatorName,
-    IsModifiableType,
-    ListTagsPaginatorName,
-    ParameterTypeType,
-    SSEStatusType,
-    SourceTypeType,
-    DAXServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_dax.literals import ChangeTypeType
 
 
 def check_value(value: ChangeTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dax.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DAX` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/type_defs/).
+
 ```python
-from types_aiobotocore_dax.type_defs import (
-    EndpointTypeDef,
-    NotificationConfigurationTypeDef,
-    ParameterGroupStatusTypeDef,
-    SSEDescriptionTypeDef,
-    SecurityGroupMembershipTypeDef,
-    SSESpecificationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateParameterGroupRequestRequestTypeDef,
-    ParameterGroupTypeDef,
-    CreateSubnetGroupRequestRequestTypeDef,
-    DecreaseReplicationFactorRequestRequestTypeDef,
-    DeleteClusterRequestRequestTypeDef,
-    DeleteParameterGroupRequestRequestTypeDef,
-    DeleteSubnetGroupRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeClustersRequestRequestTypeDef,
-    DescribeDefaultParametersRequestRequestTypeDef,
-    TimestampTypeDef,
-    EventTypeDef,
-    DescribeParameterGroupsRequestRequestTypeDef,
-    DescribeParametersRequestRequestTypeDef,
-    DescribeSubnetGroupsRequestRequestTypeDef,
-    IncreaseReplicationFactorRequestRequestTypeDef,
-    ListTagsRequestRequestTypeDef,
-    NodeTypeSpecificValueTypeDef,
-    ParameterNameValueTypeDef,
-    RebootNodeRequestRequestTypeDef,
-    SubnetTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateClusterRequestRequestTypeDef,
-    UpdateSubnetGroupRequestRequestTypeDef,
-    NodeTypeDef,
-    CreateClusterRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
-    ListTagsResponseTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
-    CreateParameterGroupResponseTypeDef,
-    DescribeParameterGroupsResponseTypeDef,
-    UpdateParameterGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
-    DescribeEventsRequestRequestTypeDef,
-    DescribeEventsResponseTypeDef,
-    ParameterTypeDef,
-    UpdateParameterGroupRequestRequestTypeDef,
-    SubnetGroupTypeDef,
-    ClusterTypeDef,
-    DescribeDefaultParametersResponseTypeDef,
-    DescribeParametersResponseTypeDef,
-    CreateSubnetGroupResponseTypeDef,
-    DescribeSubnetGroupsResponseTypeDef,
-    UpdateSubnetGroupResponseTypeDef,
-    CreateClusterResponseTypeDef,
-    DecreaseReplicationFactorResponseTypeDef,
-    DeleteClusterResponseTypeDef,
-    DescribeClustersResponseTypeDef,
-    IncreaseReplicationFactorResponseTypeDef,
-    RebootNodeResponseTypeDef,
-    UpdateClusterResponseTypeDef,
-)
+from types_aiobotocore_dax.type_defs import EndpointTypeDef
 
 
 def get_value() -> EndpointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dax-2.5.2.post1/types_aiobotocore_dax.egg-info/SOURCES.txt` & `types-aiobotocore-dax-2.5.2.post2/types_aiobotocore_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

